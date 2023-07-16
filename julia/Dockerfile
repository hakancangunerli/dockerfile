# Base image
FROM julia:latest

WORKDIR /app


RUN julia -e 'using Pkg; Pkg.activate("."); Pkg.instantiate();'


COPY . .

# Set the entrypoint command
CMD ["julia", "main.jl"]
