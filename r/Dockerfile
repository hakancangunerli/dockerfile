# Base image
FROM r-base:4.1.0

# Set the working directory
WORKDIR /app

# Copy the R project files
COPY test.R .

# Install R dependencies using renv
RUN R -e 'install.packages("renv")'
RUN R -e 'renv::init(); renv::restore()'

# Set the entrypoint command
CMD ["Rscript", "main.R"]