## Useful Methods

<pre>
  create_rectangle_from_two_clicks(debug: object) -> tuple
  Does what it says and copies a 'variable template' to your clipboard
</pre>

<pre>
  get_text_from_rectangle(rectangle: tuple, py_tess_path: str, debug: object) -> str
  Gets the text from a [RECT-'like' Object](https://learn.microsoft.com/en-us/windows/win32/api/windef/ns-windef-rect#Syntax)
</pre>

<pre>
  capture_window_area(rectangle: tuple) -> Image
  Returns an in memory screenshot (required pyscreenshot)
</pre>

<pre>
  await_found_text(
    lookFor: list[str] | str, rect: tuple, tessPath: str, trys: int = 5
  ) -> tuple[bool, int]

  Blocks execution until string/string[] is/are found
    if string[] returns (True|False, indexFound|None)
    else returns True|False
</pre>
