* Có rất nhiều công cụ phân tích sẵn có trên thị trường giúp bạn có thể khám phá, 
    ghi lại, truy cập, phân tích và xử lý các dữ liệu phi cấu trúc này. Trong số tất cả 
    có thể nhắc tới Elasticsearch là một trong những công cụ nổi bật nhất.
* Elasticsearch là công cụ tìm kiếm và lưu trữ toàn văn bản, có khả năng mở rộng cao. 
    Nó cho phép chúng ta lưu trữ, tìm kiếm và phân tích với dữ liệu rất lớn, cho kết 
    quả gần với thời gian thực. Elastic thường được sử dụng như một công cụ hỗ trợ cho 
    những app có chức năng search hoặc yêu cầu phức tạp.
* Elasticsearch là một công cụ tìm kiếm dựa trên Lucene. Nó cung cấp một công cụ 
    tìm kiếm toàn diện có khả năng phân tán, đa nhiệm với HTTP web interface và schema-free JSON documents.
* Nói cách khác, Elasticsearch là một database server mã nguồn mở, độc lập được phát triển trong Java. 
    Về cơ bản, nó được sử dụng để tìm kiếm và phân tích văn bản (full-text-search). 
    Nó lấy dữ liệu không cấu trúc từ nhiều nguồn khác nhau và lưu trữ nó ở định dạng phức tạp 
    được tối ưu hóa cao cho các tìm kiếm dựa trên ngôn ngữ.
* Elasticsearch sử dụng Apache Lucene để indexing và searching. Do đó, Lucene chỉ là một 
    thư viện và để làm việc được với nó sẽ là một quá trình rất phức tạp. Tuy nhiên, 
    Elasticsearch đã khắc phục các khó khăn đó bằng cách ẩn tất cả những thao tác phức tạp 
    bằng cách cung cấp quyền truy cập vào API. API đi kèm dưới dạng một API RESTful HTTP sử dụng JSON 
    làm định dạng trao đổi dữ liệu. Sử dụng Elasticsearch bạn có thể lưu trữ, tìm kiếm và phân tích 
    khối lượng lớn dữ liệu một cách nhanh chóng và hiệu quả. Nó đặc biệt hữu ích trong khi xử lý dữ 
    liệu bán cấu trúc tức là ngôn ngữ tự nhiên.

** Ưu điểm của Elasticsearch:

    * Khả năng mở rộng
        Elasticsearch rất dễ mở rộng và đáng tin cậy.
        Giúp đơn giản hóa các kiến trúc phức tạp và tiết kiệm thời gian trong quá trình thực hiện các dự án.

    * Tốc độ
        Elasticsearch sử dụng distributed inverted indices để tìm các kết quả phù hợp nhất cho 
        full-text searches giúp việc tìm kiếm từ các tập dữ liệu rất lớn trở nên vô cùng nhanh chóng.

    * Dễ dàng sử dụng API
        Elasticsearch cung cấp các API RESTful đơn giản và sử dụng các schema-free JSON documents 
        giúp việc indexing, searching, và querying thật dễ dàng.

    * Đa ngôn ngữ
        hỗ trợ nhiều tài liệu được viết bằng các ngôn ngữ khác nhau như tiếng Ả Rập, tiếng Braxin, tiếng Trung, 
        tiếng Anh, tiếng Pháp, tiếng Hindi, tiếng Hàn,...

    * Theo định hướng tài liệu (Document-Oriented)
        Elasticsearch lưu trữ các thực thể phức tạp trong thế giới thực dưới dạng các structured JSON 
        documents và lập chỉ mục tất cả các trường theo mặc định giúp cho dữ liệu luôn có thể tìm kiếm được. 

    * Tự động hoàn thành (autocompletion)
        Elasticsearch cung cấp chức năng tự động hoàn thành. Bằng cách dự đoán từ bằng cách sử dụng 
        rất ít ký tự, autocompletion sẽ tăng tốc độ tương tác giữa con người và máy tính.

    * Schema-Free
        Elasticsearch là schema-free vì nó chấp nhận các tài liệu JSON. Nó cố gắng phát hiện 
        cấu trúc dữ liệu, lập chỉ mục dữ liệu, làm cho dữ liệu có thể tìm kiếm được.

    ** Các khái niệm cơ bản của Elasticsearch:
        * Near Real-Time:
            nó có thể thường xuyên lên lịch cho một trạng thái mới của các tài liệu tìm kiếm được.
            mặc định các trạng thái sẽ được làm mới theo giây.
            sẽ tồn tại một độ trễ nhỏ cho đến khi tài liệu trở nên có thể tìm kiếm được, từ lúc bạn lập index
        * Index
            là tập hợp các tài liệu có đặc điểm tương tự
            một index được xác định bởi một tên duy nhất và phải là chữ thường
        * Document
            là một đơn vị thông tin cơ bản mà chúng ta có thể lập index
            bao gồm các trường khác nhau và mỗi trường trong số các trường này được xác định theo tên, 
                và có thể chứa một hoặc nhiều giá trị.
            Các tài liệu này đều là schema free và có thể có một nhóm trường khác.
            Tài liệu này là một JSON (JavaScript Object Notation).
        * Type
             type được định nghĩa cho các tài liệu có một tập các trường chung
             là một logical category/partition của một index có ngữ nghĩa học hoàn toàn tùy thuộc vào người dùng.
        * Node
            là một single instance của Elasticsearch server lưu trữ dữ liệu
            tham gia vào cluster's indexing và searching capabilities.
            một IDentifier ngẫu nhiên duy nhất (UUID) được gán cho node khi khởi động. 
            xác định máy chủ nào trong mạng của bạn tương ứng với các node nào trong cụm Elasticsearch 
                bằng cách sử dụng các tên này.
        * Cluster
            là một tập hợp của một hoặc nhiều node Elasticsearch (máy chủ) hoạt động cùng nhau
            chứa toàn bộ dữ liệu và cung cấp khả năng index và search dễ dàng trên tất cả các node, 
            cho phép xử lý dễ dàng một khối lượng dữ liệu quá lớn so với khả năng xử lý của một node duy nhất
        * Shards
            cho phép bạn chia nhỏ chỉ mục của mình thành nhiều phần được gọi là phân đoạn.
            Số lượng mảnh cần thiết có thể được xác định trong khi tạo chỉ mục
        * Replicas
            một cơ chế chuyển đổi dự phòng (failover mechanism)
            chỉ là một bản sao bổ sung của shard và có thể được sử dụng cho các truy vấn giống như bản gốc.
    
    ** Các quy ước API

        * Multiple Indices
            các hoạt động trong API dành cho nhiều chỉ mục
            thực hiện truy vấn liên quan một lần duy nhất
            Ký hiệu phân tách bằng dấu phẩy
            Ký tự đại diện (demo *, de * o2, demo3, -demo3)
            _all từ khóa cho tất cả các chỉ mục
            Tham số chuỗi truy vấn URL (ignore_unavailable, allow_no_indices, expand_wildcards)
        * Date Math Support trong Index Name
            tìm kiếm một loạt các time-series indices bằng cách sử dụng date math index name resolution
            Loại tìm kiếm này giới hạn số index đang được tìm kiếm, do đó giảm tải trên cluster 
                và cải thiện hiệu suất thực hiện
        * Common option
            As pretty ...
        * ULR-based access control
            use a proxy with URL-based access control to secure access to Elasticsearch indices,
            


