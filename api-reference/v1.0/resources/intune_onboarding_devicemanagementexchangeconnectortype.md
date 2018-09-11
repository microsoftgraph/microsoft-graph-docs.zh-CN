# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="cc618-101">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc618-101">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="cc618-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc618-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc618-103">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="cc618-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="cc618-104">成员</span><span class="sxs-lookup"><span data-stu-id="cc618-104">Members</span></span>
|<span data-ttu-id="cc618-105">成员</span><span class="sxs-lookup"><span data-stu-id="cc618-105">Member</span></span>|<span data-ttu-id="cc618-106">值</span><span class="sxs-lookup"><span data-stu-id="cc618-106">Value</span></span>|<span data-ttu-id="cc618-107">说明</span><span class="sxs-lookup"><span data-stu-id="cc618-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc618-108">onPremises</span><span class="sxs-lookup"><span data-stu-id="cc618-108">On-premises</span></span>|<span data-ttu-id="cc618-109">0</span><span class="sxs-lookup"><span data-stu-id="cc618-109">{0}</span></span>|<span data-ttu-id="cc618-110">连接到内部部署的 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="cc618-110">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="cc618-111">hosted</span><span class="sxs-lookup"><span data-stu-id="cc618-111">Hosted</span></span>|<span data-ttu-id="cc618-112">1</span><span class="sxs-lookup"><span data-stu-id="cc618-112">-1</span></span>|<span data-ttu-id="cc618-113">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="cc618-113">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="cc618-114">serviceToService</span><span class="sxs-lookup"><span data-stu-id="cc618-114">Service-to-service</span></span>|<span data-ttu-id="cc618-115">2</span><span class="sxs-lookup"><span data-stu-id="cc618-115">-2</span></span>|<span data-ttu-id="cc618-116">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="cc618-116">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="cc618-117">dedicated</span><span class="sxs-lookup"><span data-stu-id="cc618-117">Dedicated</span></span>|<span data-ttu-id="cc618-118">3</span><span class="sxs-lookup"><span data-stu-id="cc618-118">-3</span></span>|<span data-ttu-id="cc618-119">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="cc618-119">Connects to O365 Dedicated Exchange environment.</span></span>|








