## Useful Methods

<pre>
  create_rectangle_from_two_clicks(debug: object) -> tuple
</pre>
  Does what it says and copies a 'variable template' to your clipboard

<pre>
  get_text_from_rectangle(rectangle: tuple, py_tess_path: str, debug: object) -> str
</pre>
  Gets the text from a [RECT-'like' Object](https://learn.microsoft.com/en-us/windows/win32/api/windef/ns-windef-rect#Syntax)

<pre>
  capture_window_area(rectangle: tuple) -> Image
</pre>
  Returns an in memory screenshot (required pyscreenshot)

<pre>
  await_found_text(
    lookFor: list[str] | str, rect: tuple, tessPath: str, trys: int = 5
  ) -> tuple[bool, int]
</pre>
  Blocks execution until string/string[] is/are found <br/>
      - if string[] returns (True|False, indexFound|None) <br/>
      - else returns True|False
