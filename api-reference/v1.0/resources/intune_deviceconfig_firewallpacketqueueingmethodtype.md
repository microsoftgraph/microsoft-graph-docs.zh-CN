# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="5a041-101">firewallPacketQueueingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5a041-101">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="5a041-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5a041-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a041-103">FirewallPacketQueueingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="5a041-103">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="5a041-104">成员</span><span class="sxs-lookup"><span data-stu-id="5a041-104">Members</span></span>
|<span data-ttu-id="5a041-105">成员</span><span class="sxs-lookup"><span data-stu-id="5a041-105">Member</span></span>|<span data-ttu-id="5a041-106">值</span><span class="sxs-lookup"><span data-stu-id="5a041-106">Value</span></span>|<span data-ttu-id="5a041-107">说明</span><span class="sxs-lookup"><span data-stu-id="5a041-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a041-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5a041-108">deviceDefault</span></span>|<span data-ttu-id="5a041-109">0</span><span class="sxs-lookup"><span data-stu-id="5a041-109">{0}</span></span>|<span data-ttu-id="5a041-110">没有由 Intune 配置的值，不要替代用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="5a041-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="5a041-111">disabled</span><span class="sxs-lookup"><span data-stu-id="5a041-111">disabled</span></span>|<span data-ttu-id="5a041-112">1</span><span class="sxs-lookup"><span data-stu-id="5a041-112">-1</span></span>|<span data-ttu-id="5a041-113">禁用数据包的队列</span><span class="sxs-lookup"><span data-stu-id="5a041-113">Disable packet queuing</span></span>|
|<span data-ttu-id="5a041-114">queueInbound</span><span class="sxs-lookup"><span data-stu-id="5a041-114">queueInbound</span></span>|<span data-ttu-id="5a041-115">2</span><span class="sxs-lookup"><span data-stu-id="5a041-115">-2</span></span>|<span data-ttu-id="5a041-116">队列入站加密数据包</span><span class="sxs-lookup"><span data-stu-id="5a041-116">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="5a041-117">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="5a041-117">queueOutbound</span></span>|<span data-ttu-id="5a041-118">3</span><span class="sxs-lookup"><span data-stu-id="5a041-118">-3</span></span>|<span data-ttu-id="5a041-119">队列解密出站数据包以进行转发</span><span class="sxs-lookup"><span data-stu-id="5a041-119">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="5a041-120">queueBoth</span><span class="sxs-lookup"><span data-stu-id="5a041-120">queueBoth</span></span>|<span data-ttu-id="5a041-121">4</span><span class="sxs-lookup"><span data-stu-id="5a041-121">-4</span></span>|<span data-ttu-id="5a041-122">队列入站和出站数据包</span><span class="sxs-lookup"><span data-stu-id="5a041-122">Queue both inbound and outbound packets</span></span>|








