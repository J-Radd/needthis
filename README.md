# needthis
StripeConfiguration.ApiKey = "sk_test_51HmuxwJtofXoPBKRajCQr5ivlqKmbMz5uDKBWXXyRQl27rsr2zbEdAkJgVt1VVBbI80gT4ir68E7dcsvchVOqPJE00zubKlhIv";

var options = new AccountCreateOptions
{
  Type = "express",
};

var service = new AccountService();
var account = service.Create(options);
// Set your secret key. Remember to switch to your live secret key in production!
// See your keys here: https://dashboard.stripe.com/account/apikeys
StripeConfiguration.ApiKey = "sk_test_51HmuxwJtofXoPBKRajCQr5ivlqKmbMz5uDKBWXXyRQl27rsr2zbEdAkJgVt1VVBbI80gT4ir68E7dcsvchVOqPJE00zubKlhIv";

var options = new AccountLinkCreateOptions
{
    Account = "acct_1032D82eZvKYlo2C",
    RefreshUrl = "https://example.com/reauth",
    ReturnUrl = "https://example.com/return",
    Type = "account_onboarding",
};
var service = new AccountLinkService();
var accountLink = service.Create(options);

