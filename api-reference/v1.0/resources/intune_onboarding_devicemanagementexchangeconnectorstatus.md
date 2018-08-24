# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="22975-101">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="22975-101">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="22975-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="22975-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22975-103">Exchange 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="22975-103">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="22975-104">成员</span><span class="sxs-lookup"><span data-stu-id="22975-104">Members</span></span>
|<span data-ttu-id="22975-105">成员</span><span class="sxs-lookup"><span data-stu-id="22975-105">Member</span></span>|<span data-ttu-id="22975-106">值</span><span class="sxs-lookup"><span data-stu-id="22975-106">Value</span></span>|<span data-ttu-id="22975-107">说明</span><span class="sxs-lookup"><span data-stu-id="22975-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22975-108">none</span><span class="sxs-lookup"><span data-stu-id="22975-108">none</span></span>|<span data-ttu-id="22975-109">0</span><span class="sxs-lookup"><span data-stu-id="22975-109">{0}</span></span>|<span data-ttu-id="22975-110">没有连接器存在。</span><span class="sxs-lookup"><span data-stu-id="22975-110">No Connector exists.</span></span>|
|<span data-ttu-id="22975-111">connectionPending</span><span class="sxs-lookup"><span data-stu-id="22975-111">connectionPending</span></span>|<span data-ttu-id="22975-112">1</span><span class="sxs-lookup"><span data-stu-id="22975-112">-1</span></span>|<span data-ttu-id="22975-113">待连接到 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="22975-113">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="22975-114">connected</span><span class="sxs-lookup"><span data-stu-id="22975-114">Connected</span></span>|<span data-ttu-id="22975-115">2</span><span class="sxs-lookup"><span data-stu-id="22975-115">-2</span></span>|<span data-ttu-id="22975-116">已连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="22975-116">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="22975-117">disconnected</span><span class="sxs-lookup"><span data-stu-id="22975-117">disconnected</span></span>|<span data-ttu-id="22975-118">3</span><span class="sxs-lookup"><span data-stu-id="22975-118">-3</span></span>|<span data-ttu-id="22975-119">从 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="22975-119">Disconnected from the Exchange Environment</span></span>|



