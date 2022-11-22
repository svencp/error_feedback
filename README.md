# error feedback
formatted strings on error feedback 


    #[test]
    fn t001_underline() {
        let s = justify("Hello Svenny!".to_string(), 40, Justify::Center);
        underline_string(s.clone());
        print!("\n");
        let len = s.clone().len();

        assert_eq!(len, 40);
    }
    
    #[test]
    fn t002_justify() {
        let s = justify("1.5y".to_string(), 7, Justify::Right);
        assert_eq!(s.len(), 7);
    }




