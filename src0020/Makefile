# 
# make file
# 
CXX         = g++
CXXFLAG     = $(CXXINCLUDE)
CXXINCLUDE  =
# プロジェクトのターゲット名
TARGET 		= 
DEBUG       =
## DEBUG    =   -g
# オブジェクトファイルの定義
OBJS = $(SRCS:.cpp=.o)

all:
	$(TARGET)

g++: 
#コンパイル
	g++ -c mylib.cpp -o mylib.o
	g++ -c submain.cpp -o submain.o
#リンク
	g++ submain.o mylib.o -o out

clean:
	-rm -f $(OBJS) $(TARGET) *.o *.exe
	