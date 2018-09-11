# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="ebef5-101">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ebef5-101">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="ebef5-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ebef5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebef5-103">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="ebef5-103">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="ebef5-104">成员</span><span class="sxs-lookup"><span data-stu-id="ebef5-104">Members</span></span>
|<span data-ttu-id="ebef5-105">成员</span><span class="sxs-lookup"><span data-stu-id="ebef5-105">Member</span></span>|<span data-ttu-id="ebef5-106">值</span><span class="sxs-lookup"><span data-stu-id="ebef5-106">Value</span></span>|<span data-ttu-id="ebef5-107">说明</span><span class="sxs-lookup"><span data-stu-id="ebef5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebef5-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ebef5-108">notConfigured</span></span>|<span data-ttu-id="ebef5-109">0</span><span class="sxs-lookup"><span data-stu-id="ebef5-109">{0}</span></span>|<span data-ttu-id="ebef5-110">默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强大的检测, 而不增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="ebef5-110">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="ebef5-111">high</span><span class="sxs-lookup"><span data-stu-id="ebef5-111">High.</span></span>|<span data-ttu-id="ebef5-112">1</span><span class="sxs-lookup"><span data-stu-id="ebef5-112">-1</span></span>|<span data-ttu-id="ebef5-113">High应用了强大的检测级别。</span><span class="sxs-lookup"><span data-stu-id="ebef5-113">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="ebef5-114">highPlus</span><span class="sxs-lookup"><span data-stu-id="ebef5-114">highPlus</span></span>|<span data-ttu-id="ebef5-115">2</span><span class="sxs-lookup"><span data-stu-id="ebef5-115">-2</span></span>|<span data-ttu-id="ebef5-116">高 + 使用的高级别和应用加法保护措施</span><span class="sxs-lookup"><span data-stu-id="ebef5-116">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="ebef5-117">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="ebef5-117">zeroTolerance</span></span>|<span data-ttu-id="ebef5-118">3</span><span class="sxs-lookup"><span data-stu-id="ebef5-118">-3</span></span>|<span data-ttu-id="ebef5-119">零公差阻止所有未知的可执行文件</span><span class="sxs-lookup"><span data-stu-id="ebef5-119">Zero tolerance blocks all unknown executables</span></span>|








