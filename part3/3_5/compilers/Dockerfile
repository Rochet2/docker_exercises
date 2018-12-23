FROM mono:4-onbuild

# RUN useradd -m app
# RUN chown -R app /usr/src/app/build
# USER app

CMD ["mono", "./Interpreter.exe"]

# docker build -t compilers2 .
# docker run --rm -v $(pwd)/code.txt:/usr/src/app/build/code.txt:ro compilers2 mono ./Interpreter.exe code.txt
