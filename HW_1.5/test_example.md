pm.test("Body is correct", function ()  {


pm.test("Body matches string", function () {






const paramsString = request.url.split('?')[1];
const eachParamArray = paramsString.split('&');
let params = {};
eachParamArray.forEach((param) => {
    const key = param.split('=')[0];
    const value = param.split('=')[1];
    Object.assign(params, {[key]: value});
});
console.log(params);

let a = pm.request.url.query.all()

pm.expect(jsonData.family.pets.dog).to.have.property("name")