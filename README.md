public class Accccoun {
 public static void method(){
        http h=new http();
        httpRequest req=new httpRequest();
        req.setEndpoint('Callout:Currncy_Convertor'+'/api/latest?access_key='1999a56e9b6f1a18c25af4a433e7372a');
        req.setMethod('GET');
        httpResponse res=h.send(req);
        System.debug('Results:'+res.getBody());
        Map<string,Object> ll=(Map<string,Object>)JSON.deserializeUntyped(res.getBody());	
        System.debug('lll : '+ll);
    }
    
 }
