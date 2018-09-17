# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="e80bf-101">deviceManagementExchangeConnectorSyncType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e80bf-101">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="e80bf-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e80bf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e80bf-103">请求 Exchange Connector 同步的类型。</span><span class="sxs-lookup"><span data-stu-id="e80bf-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="e80bf-104">成员</span><span class="sxs-lookup"><span data-stu-id="e80bf-104">Members</span></span>
|<span data-ttu-id="e80bf-105">成员</span><span class="sxs-lookup"><span data-stu-id="e80bf-105">Member</span></span>|<span data-ttu-id="e80bf-106">值</span><span class="sxs-lookup"><span data-stu-id="e80bf-106">Value</span></span>|<span data-ttu-id="e80bf-107">说明</span><span class="sxs-lookup"><span data-stu-id="e80bf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e80bf-108">fullSync</span><span class="sxs-lookup"><span data-stu-id="e80bf-108">fullSync</span></span>|<span data-ttu-id="e80bf-109">0</span><span class="sxs-lookup"><span data-stu-id="e80bf-109">{0}</span></span>|<span data-ttu-id="e80bf-110">发现 Exchange 中的所有设备。</span><span class="sxs-lookup"><span data-stu-id="e80bf-110">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="e80bf-111">deltaSync</span><span class="sxs-lookup"><span data-stu-id="e80bf-111">deltaSync</span></span>|<span data-ttu-id="e80bf-112">1</span><span class="sxs-lookup"><span data-stu-id="e80bf-112">-1</span></span>|<span data-ttu-id="e80bf-113">在 Exchange 中仅发现在增量同步窗口期间已更新的设备。</span><span class="sxs-lookup"><span data-stu-id="e80bf-113">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|








