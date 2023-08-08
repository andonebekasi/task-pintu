# Use the official Go image as the base image
FROM golang:latest

# Set the working directory inside the container
WORKDIR /app

# Copy the Go application files into the container
COPY . .

# Build the Go application
RUN go build -o webapp main.go

# Expose port 8080
EXPOSE 8080

# Start the Go application when the container runs
CMD ["./webapp"]
