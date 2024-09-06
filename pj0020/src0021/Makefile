# コンパイラとフラグの定義
CXX = g++
CXXFLAGS = -Wall -g

# プロジェクトのターゲット名
TARGET = out

# ソースファイルとヘッダーファイルの定義
SRCS =  submain.cpp mylib.cpp
HEADERS = mylib.h

# オブジェクトファイルの定義
OBJS = $(SRCS:.cpp=.o)

$(TARGET): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(OBJS)

# 各ソースファイルからオブジェクトファイルを作成するルール
%.o: %.cpp $(HEADERS)
	$(CXX) $(CXXFLAGS) -c $<

# クリーンアップルール
clean:
	rm -f $(OBJS) $(TARGET) 
