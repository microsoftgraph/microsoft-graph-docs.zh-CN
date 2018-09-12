# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="55cf6-101">androidWorkProfileRequiredPasswordType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55cf6-101">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="55cf6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55cf6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55cf6-103">Android 工作配置文件所需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="55cf6-103">Android Work Profile required password type.</span></span>
## <a name="members"></a><span data-ttu-id="55cf6-104">成员</span><span class="sxs-lookup"><span data-stu-id="55cf6-104">Members</span></span>
|<span data-ttu-id="55cf6-105">成员</span><span class="sxs-lookup"><span data-stu-id="55cf6-105">Member</span></span>|<span data-ttu-id="55cf6-106">值</span><span class="sxs-lookup"><span data-stu-id="55cf6-106">Value</span></span>|<span data-ttu-id="55cf6-107">说明</span><span class="sxs-lookup"><span data-stu-id="55cf6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55cf6-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="55cf6-108">deviceDefault</span></span>|<span data-ttu-id="55cf6-109">0</span><span class="sxs-lookup"><span data-stu-id="55cf6-109">{0}</span></span>|<span data-ttu-id="55cf6-110">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="55cf6-110">Device default value, no intent.</span></span>|
|<span data-ttu-id="55cf6-111">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="55cf6-111">lowSecurityBiometric</span></span>|<span data-ttu-id="55cf6-112">1</span><span class="sxs-lookup"><span data-stu-id="55cf6-112">-1</span></span>|<span data-ttu-id="55cf6-113">需要低安全性的基于生物的密码。</span><span class="sxs-lookup"><span data-stu-id="55cf6-113">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="55cf6-114">required</span><span class="sxs-lookup"><span data-stu-id="55cf6-114">required</span></span>|<span data-ttu-id="55cf6-115">2</span><span class="sxs-lookup"><span data-stu-id="55cf6-115">-2</span></span>|<span data-ttu-id="55cf6-116">必需。</span><span class="sxs-lookup"><span data-stu-id="55cf6-116">Required.</span></span>|
|<span data-ttu-id="55cf6-117">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="55cf6-117">atLeastNumeric</span></span>|<span data-ttu-id="55cf6-118">3</span><span class="sxs-lookup"><span data-stu-id="55cf6-118">-3</span></span>|<span data-ttu-id="55cf6-119">必需至少是数字密码。</span><span class="sxs-lookup"><span data-stu-id="55cf6-119">At least numeric password required.</span></span>|
|<span data-ttu-id="55cf6-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="55cf6-120">numericComplex</span></span>|<span data-ttu-id="55cf6-121">4</span><span class="sxs-lookup"><span data-stu-id="55cf6-121">-4</span></span>|<span data-ttu-id="55cf6-122">必需是复杂的数字密码。</span><span class="sxs-lookup"><span data-stu-id="55cf6-122">Numeric complex password required.</span></span>|
|<span data-ttu-id="55cf6-123">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="55cf6-123">atLeastAlphabetic</span></span>|<span data-ttu-id="55cf6-124">5</span><span class="sxs-lookup"><span data-stu-id="55cf6-124">-5</span></span>|<span data-ttu-id="55cf6-125">必需至少是字母密码。</span><span class="sxs-lookup"><span data-stu-id="55cf6-125">At least alphabetic password required.</span></span>|
|<span data-ttu-id="55cf6-126">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="55cf6-126">atLeastAlphanumeric</span></span>|<span data-ttu-id="55cf6-127">6</span><span class="sxs-lookup"><span data-stu-id="55cf6-127">-6</span></span>|<span data-ttu-id="55cf6-128">必需至少是字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="55cf6-128">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="55cf6-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="55cf6-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="55cf6-130">7</span><span class="sxs-lookup"><span data-stu-id="55cf6-130">-7</span></span>|<span data-ttu-id="55cf6-131">必需至少是带符号的字母数字密码。</span><span class="sxs-lookup"><span data-stu-id="55cf6-131">At least alphanumeric with symbols password required.</span></span>|








