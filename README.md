# needthis
StripeConfiguration.ApiKey = "sk_test_51HmuxwJtofXoPBKRajCQr5ivlqKmbMz5uDKBWXXyRQl27rsr2zbEdAkJgVt1VVBbI80gT4ir68E7dcsvchVOqPJE00zubKlhIv";

var options = new AccountCreateOptions
{
  Type = "express",
};

var service = new AccountService();
var account = service.Create(options);

