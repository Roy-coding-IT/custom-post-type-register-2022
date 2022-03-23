# custom-post-type-register-2022

function saurav_theme_custom_posts(){
                register_post_type('slide/name', array(
                
                    'public'      => true,
                    'label'       => 'Slider',
                    'labels'       => array(
                        
                        'name'      => 'slides',
                        'singular_name'  => 'slide',
                        'add_new'      => 'Add new Slide',
                    ),
                    'supports' => array('title', 'editor', 'thumbnail', 'excerpt')
                    
                ));
    
    
}

add_action( 'init', 'saurav_theme_custom_posts' );
