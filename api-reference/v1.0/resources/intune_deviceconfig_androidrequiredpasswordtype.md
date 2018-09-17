# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="d052a-101">androidRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d052a-101">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="d052a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d052a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d052a-103">Android 所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d052a-103">The required password type.</span></span>
## <a name="members"></a><span data-ttu-id="d052a-104">成员</span><span class="sxs-lookup"><span data-stu-id="d052a-104">Members</span></span>
|<span data-ttu-id="d052a-105">成员</span><span class="sxs-lookup"><span data-stu-id="d052a-105">Member</span></span>|<span data-ttu-id="d052a-106">值</span><span class="sxs-lookup"><span data-stu-id="d052a-106">Value</span></span>|<span data-ttu-id="d052a-107">说明</span><span class="sxs-lookup"><span data-stu-id="d052a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d052a-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d052a-108">deviceDefault</span></span>|<span data-ttu-id="d052a-109">0</span><span class="sxs-lookup"><span data-stu-id="d052a-109">{0}</span></span>|<span data-ttu-id="d052a-110">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="d052a-110">Device default value, no intent.</span></span>|
|<span data-ttu-id="d052a-111">alphabetic</span><span class="sxs-lookup"><span data-stu-id="d052a-111">alphabetic</span></span>|<span data-ttu-id="d052a-112">1</span><span class="sxs-lookup"><span data-stu-id="d052a-112">-1</span></span>|<span data-ttu-id="d052a-113">必需是字母密码。</span><span class="sxs-lookup"><span data-stu-id="d052a-113">Alphabetic password required.</span></span>|
|<span data-ttu-id="d052a-114">alphanumeric</span><span class="sxs-lookup"><span data-stu-id="d052a-114">alphanumeric</span></span>|<span data-ttu-id="d052a-115">2</span><span class="sxs-lookup"><span data-stu-id="d052a-115">-2</span></span>|<span data-ttu-id="d052a-116">必须是字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d052a-116">Alphanumeric password required</span></span>|
|<span data-ttu-id="d052a-117">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d052a-117">alphanumericWithSymbols</span></span>|<span data-ttu-id="d052a-118">3</span><span class="sxs-lookup"><span data-stu-id="d052a-118">-3</span></span>|<span data-ttu-id="d052a-119">必需是带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="d052a-119">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="d052a-120">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="d052a-120">lowSecurityBiometric</span></span>|<span data-ttu-id="d052a-121">4</span><span class="sxs-lookup"><span data-stu-id="d052a-121">-4</span></span>|<span data-ttu-id="d052a-122">需要低安全性的基于生物的密码。</span><span class="sxs-lookup"><span data-stu-id="d052a-122">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="d052a-123">numeric</span><span class="sxs-lookup"><span data-stu-id="d052a-123">Numeric</span></span>|<span data-ttu-id="d052a-124">5</span><span class="sxs-lookup"><span data-stu-id="d052a-124">-5</span></span>|<span data-ttu-id="d052a-125">必需数字密码。</span><span class="sxs-lookup"><span data-stu-id="d052a-125">Numeric password required.</span></span>|
|<span data-ttu-id="d052a-126">numericComplex</span><span class="sxs-lookup"><span data-stu-id="d052a-126">numericComplex</span></span>|<span data-ttu-id="d052a-127">6</span><span class="sxs-lookup"><span data-stu-id="d052a-127">-6</span></span>|<span data-ttu-id="d052a-128">必需是复杂的数字密码。</span><span class="sxs-lookup"><span data-stu-id="d052a-128">Numeric complex password required.</span></span>|
|<span data-ttu-id="d052a-129">any</span><span class="sxs-lookup"><span data-stu-id="d052a-129">any</span></span>|<span data-ttu-id="d052a-130">7</span><span class="sxs-lookup"><span data-stu-id="d052a-130">-7</span></span>|<span data-ttu-id="d052a-131">Password 或模式是必需的且可接受任何形式。</span><span class="sxs-lookup"><span data-stu-id="d052a-131">A password or pattern is required, and any is acceptable.</span></span>|








