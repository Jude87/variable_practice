# variable_practice

import java.util.Scanner;

public class VariablePractice {
	public void method1() {
		//문제 1 초기화 및 값 변경
		int inum = 100;
		double dnum = 234.567;
		char ch = 'A';
		String str = "Hello World";
		boolean bool = true;
		
		System.out.println("초기화 후 : " + inum + ", " + dnum + ", " + ch + ", " + str + ", " +
							bool);
		
		inum = 10000;
		dnum = 567.123456789; // 실수형을 flaot으로 지정하면 유효자리수가 7자리라 데이터가 손실됨
		ch = 'B';
		str = "Welcome to JAVA";
		bool = false;
		
		System.out.println("값 변경 후 : " + inum + ", " + dnum + ", " + ch + ", " + str + ", " +
							bool);
		}
	public void meghod2() {
		//문제 2 원의 둘레와 면적 구하기
		Scanner sc = new Scanner(System.in);
		System.out.print("원의 반지름 입력 : ");
		int rad  = sc.nextInt(); // 스캐너에서 입력받은 정수값이 inum에 들어오도록 함
		
		System.out.println("반지름이 5인 원의 둘레 : " + 2*rad*Math.PI);
		System.out.println("반지름이 5인 원의 면적 : " + rad*rad*Math.PI);
		
		//소수점 아래 한자리까지만 표시되도록 바꿈
		System.out.printf("반지름이 %d인 원의 둘레 : %.1f\n", rad, 2*rad*Math.PI);
		System.out.printf("반지름이 %d인 원의 면적 : %.1f\n", rad, rad*rad*Math.PI);
		
		// *출력메소드
		// System.out.printf("%형식", 변수 등) f는 포멧의 f임
		// 정해져 있는 형식에 맞춰서 그 형식에 맞는 값(변수)를 줄바꿈 하지 않고 출력
		// %d : 정수형 / %o : 8진수 / %x : 16진수
		// %c : 문자 / %s : 문자열
		// %f : 실수(소수점 아래 6자리) / %e : 지수형태표현 / %g : 대입 값 그대로
		// %A : 16진수 실수
		// %b : 논리형
		
		// 정렬방법
		// %5d : 5칸을 확보하고 오른쪽 정렬
		// %-5d : 5칸을 확보하고 왼쪽 정렬
		// %.2f : 소수점 아래 2자리까지만 표시
		// \n : 역슬레시 n은 개행
		
		
	}
}
