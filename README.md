># 스파크
>```
>인메모리 기반의 대용량 데이터 고속 처리 엔진
>범용 분산 클러스터 컴퓨팅 프레임워크
>```
>
>RDD(Resilient Distributed Data) : 변경불가 분산 데이터
>```
>- 변환(Transformation) : RDD -> RDD (연산X)
>   map(), filter(), distinct(), ...
>
>- 실행(Action) : RDD -> Data (연산O)
>   collect(), count(), ...
>
>→ 분산 데이터셋, 연산 제어 코드 작성 어려움
>```
>
>데이터셋(DataSet) : 분산된 데이터 콜렉션(=데이터프레임: RDD 테이블)
>```
>- 데이터 -> 스키마(=데이터프레임 속성, 속성_타입)
>- 속도 증가
>- 데이터 자료형 검사, 직렬화
>```
```angular2html
from pyspark.sql import SparkSession
from pyspark.sql.types import StructType

import pyspark.sql.functions as F
```
