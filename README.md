#include <ncurses/ncurses.h>
#include <windows.h>
using namespace std;

int main(){
	initscr();
	
	for (int i=0; i<3; i++) {
		mvprintw(26, 100, "LOADING...");
		mvprintw(27, 100, "--------------------");
		mvprintw(28, 100, "|                  |");
		mvprintw(29, 100, "--------------------");
		
		for (int f=1; f<18; f++){
			mvprintw(28, 100 + f, "~~");
			refresh();
			Sleep(200);
			
		}
	}
	
	endwin();
	return 0;
}
