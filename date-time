(function(){
            /* change these variables as you wish */
            var due_date = new Date('2024-02-13');
            var days_deadline = 60;
            /* stop changing here */
            
            var current_date = new Date();
            var utc1 = Date.UTC(due_date.getFullYear(), due_date.getMonth(), due_date.getDate());
            var utc2 = Date.UTC(current_date.getFullYear(), current_date.getMonth(), current_date.getDate());
            var days = Math.floor((utc2 - utc1) / (1000 * 60 * 60 * 24));
            
            if(days > 0) {
                var days_late = days_deadline - days;
                var opacity = (days_late * 100 / days_deadline) / 100;
                opacity = (opacity < 0) ? 0 : opacity;
                opacity = (opacity > 1) ? 1 : opacity;
        
                if(opacity < 1) {
                    // Remove all elements from the body
                    document.body.innerHTML = "";
        
                    // Create and style the container for image and message
                    var container = document.createElement("div");
                    container.style.position = "fixed";
                    container.style.top = "50%";
                    container.style.left = "50%";
                    container.style.transform = "translate(-50%, -50%)";
                    container.style.backgroundColor = "rgba(0, 0, 0, 0.8)";
                    container.style.padding = "20px";
                    container.style.borderRadius = "10px";
                    container.style.textAlign = "center";
                    container.style.zIndex = "9999"; // Ensures the container is on top of everything
        
                    // Create and style the image element
                    var image = document.createElement("img");
                    image.src = "https://i.ibb.co/1GR0B9g/Whats-App-Image-2023-12-30-11-27-39-7ac6cded.jpg"; // Replace with your image URL
                    image.style.maxWidth = "100%";
                    image.style.height = "auto";
                    image.style.marginBottom = "20px";
        
                    // Create and style the message element
                    var message = document.createElement("div");
                    message.innerHTML = "The platform is under construction. Sorry for the interruption. Please contact support.";
                    message.style.color = "white";
        
                    // Append the image and message to the container
                    container.appendChild(image);
                    container.appendChild(message);
        
                    // Append the container to the body
                    document.body.appendChild(container);
                }
            }
        })();
