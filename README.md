# Tạo chatbot đơn giản

Hai hướng tiếp cận chính:

- Retrieval based: Hướng tiếp cận này sẽ truy vấn câu trả lời từ một tập các câu trả lời được định nghĩa trước. Không yêu cầu hiểu câu ý nghĩa của câu.
- Task oriented: Yêu cầu hiểu ý nghĩa của câu (ý định và các thực thể trong câu) để xử lý riêng cho từng trường hợp.

## Retrieval based

![picture](https://github.com/nguyenvulebinh/shecode20/blob/master/retrieval_approach.png?raw=true)

### Biểu diễn văn bản dưới dạng vector
Phương pháp đơn giản nhất là sử dụng Bag of Word (BoW) (Túi đựng Từ). BoW sẽ biểu diễn một văn bản dưới dạng một tập V các từ (V là toàn bộ từ trong từ điển) và bỏ qua các thông tin về trật tự của từ và ngữ pháp. Lấy ví dụ tập dữ liệu gồm 2 câu: 

- Bình thích xem phim. Linh cũng thích xem phim
- Bình cũng thích xem đá bóng

Dựa trên tập dữ liệu này, ta có thể xây dựng được tập từ điển gồm có các từ sau (bỏ qua việc viết hoa): {bình, linh, thích, xem, phim, cũng, đá, bóng}

Hai câu trong tập dữ liệu sẽ được biểu diễn dưới dạng vector theo BoW như sau:

- [1, 1, 2, 2, 2, 1, 0, 0]
- [1, 0, 1, 1, 0, 1, 1, 1]

## Task oriented

![picture](https://github.com/nguyenvulebinh/shecode20/blob/master/task_oriented_flow.png?raw=true)


## Kết quả 

![picture](https://github.com/nguyenvulebinh/shecode20/blob/master/chatbot_demo.png?raw=true)

Link play around in [colab](https://colab.research.google.com/drive/1_KQkMqh6zxqUXO-Y9jzmqQ7efhAUfzaI?usp=sharing)
