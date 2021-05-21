for(Map.Entry<String,TreeMap<String,TreeMap<String,ArrayList<String>>>> en:tm.entrySet()){
	System.out.print(en.getKey()+"-->");
	TreeMap<String,TreeMap<String,ArrayList<String>>> tm1=en.getValue();
	for(Map.Entry<String,TreeMap<String,ArrayList<String>>> en1:tm1.entrySet()){
		System.out.print(en1.getKey()+"-->");
		TreeMap<String,ArrayList<String>> tm2=en1.getValue();
		for(Map.Entry<String,ArrayList<String>> en2:tm2.entrySet()){
		System.out.print(en2.getKey()+"-->");
				ArrayList<String> ar=en2.getValue();
				for(int i=0;i<ar.size();i++){
					System.out.print(ar.get(i)+"->");
				}
		}
	}
}
