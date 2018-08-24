# <a name="runstate-enum-type"></a><span data-ttu-id="6a753-101">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6a753-101">runState enum type</span></span>

> <span data-ttu-id="6a753-102">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a753-102">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a753-103">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a753-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a753-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a753-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a753-105">指示设备管理脚本执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="6a753-105">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="6a753-106">成员</span><span class="sxs-lookup"><span data-stu-id="6a753-106">Members</span></span>
|<span data-ttu-id="6a753-107">成员</span><span class="sxs-lookup"><span data-stu-id="6a753-107">Member</span></span>|<span data-ttu-id="6a753-108">值</span><span class="sxs-lookup"><span data-stu-id="6a753-108">Value</span></span>|<span data-ttu-id="6a753-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a753-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a753-110">unknown</span><span class="sxs-lookup"><span data-stu-id="6a753-110">unknown</span></span>|<span data-ttu-id="6a753-111">0</span><span class="sxs-lookup"><span data-stu-id="6a753-111">{0}</span></span>|<span data-ttu-id="6a753-112">未知结果。</span><span class="sxs-lookup"><span data-stu-id="6a753-112">Unknown result.</span></span>|
|<span data-ttu-id="6a753-113">success</span><span class="sxs-lookup"><span data-stu-id="6a753-113">success</span></span>|<span data-ttu-id="6a753-114">1</span><span class="sxs-lookup"><span data-stu-id="6a753-114">-1</span></span>|<span data-ttu-id="6a753-115">脚本运行成功。</span><span class="sxs-lookup"><span data-stu-id="6a753-115">Script is run successfully.</span></span>|
|<span data-ttu-id="6a753-116">fail</span><span class="sxs-lookup"><span data-stu-id="6a753-116">Fail</span></span>|<span data-ttu-id="6a753-117">2</span><span class="sxs-lookup"><span data-stu-id="6a753-117">-2</span></span>|<span data-ttu-id="6a753-118">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="6a753-118">Script failed to run.</span></span>|



