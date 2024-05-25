# Namsan Garden Wordcloud

## Overview

남산 야외식물원의 구글 지도 리뷰를 바탕으로 워드클라우드를 생성합니다.

## Features

### csv_refine

csv 파일에서 원하는 column을 선별하여 별도의 파일로 저장한다.

- 최초 데이터

| place_id                    | place_name      | review_id    | rating | review_text                    | published_at | published_at_date | response_from_owner_text | response_from_owner_ago | response_from_owner_date | review_likes_count | total_number_of_reviews_by_reviewer | total_number_of_photos_by_reviewer | is_local_guide | review_translated_text | response_from_owner_translated_text |
| --------------------------- | --------------- | ------------ | ------ | ------------------------------ | ------------ | ----------------- | ------------------------ | ----------------------- | ------------------------ | ------------------ | ----------------------------------- | ---------------------------------- | -------------- | ---------------------- | ----------------------------------- |
| ChIJxzBkuFKifDURKFJQ7yQP-iI | 남산 야외식물원 | 1q2W3e4R5t6Y | 5      | 가족과 함께 방문하기 참 좋아요 | 4년 전       |                   |                          |                         |                          | 0                  | 10                                  | 16                                 | True           |                        |                                     |

- 수정 데이터

| published_at | review_text                    |
| ------------ | ------------------------------ |
| 2달 전       | 가족과 함께 방문하기 참 좋아요 |

### review_to_wordcloud

리뷰를 바탕으로 워드클라우드를 생성한다.
생성한 이미지를 파일로 저장한다.

- 결과
  ![result](/asset/namsan_wordcloud.png)
