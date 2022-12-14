- 👋 Hi, I’m @thuypt8511
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
thuypt8511/thuypt8511 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
phụ trợ / tài nguyên / lượt xem / chủ đề / sub_topic.blade.php
@@ -47,14 +47,8 @@
                        </nút>

                        @if (session()->get('level') === 1)

                            <form action="{{route('topics.destroy_sub_topic', ['topic' => $sub_topic->id])}}" method="post" style="float:left; ">
                                @method('XÓA')
                                @csrf
                                <nút class = "btn btn-xs btn-nguy hiểm">
                                    <i class="ace-icon fa fa-trash-o bigger-120"></i>
                                </nút>
                            </dạng>
                            <button type="button" class="btn btn-xs btn-danger" data-toggle="modal" data-target="#myModal{{$sub_topic->id}}"> <i class="ace-icon fa fa-trash-o  lớn hơn-120 ">< / i>
                            </nút>
                        @endif

                    </Div>
@@ -95,11 +89,35 @@
                </Div>
                </Td>
            </Tr>

            <div class="modal fade" id="myModal{{$sub_topic->id}}" role="dialog">
                <div class = "hộp thoại phương thức">

                    <!-- Nội dung phương thức-->
                    <div class = "modal-content">
                        <div class = "modal-header">
                            <loại nút = "nút" class = "đóng" data-disdismiss = "modal"> &times; </nút>
                            < h4 class="modal-title">Cảnh báo</h4>
                        </Div>
                        <div class = "modal-body">
                            <p>Xóa danh mục này sẽ xóa tất cả bài viết thuộc danh mục này</p>
                        </Div>
                        <div class = "modal-footer">
                            <form action="{{route('topics.destroy_sub_topic', ['topic' => $sub_topic->id])}}" method="post">
                                @method('XÓA')
                                @csrf
                                <button type="submit" class="btn btn-danger">Xóa</nút>
                            </dạng>
                        </Div>
                    </Div>

                </Div>
            </Div>

        @endforeach

        </vật thể>
    </bàn>



@endsection
