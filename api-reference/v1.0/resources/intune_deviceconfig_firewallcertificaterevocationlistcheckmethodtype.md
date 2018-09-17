# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="096c1-101">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="096c1-101">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="096c1-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="096c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="096c1-103">firewallCertificateRevocationListCheckMethod 可能的值</span><span class="sxs-lookup"><span data-stu-id="096c1-103">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="096c1-104">成员</span><span class="sxs-lookup"><span data-stu-id="096c1-104">Members</span></span>
|<span data-ttu-id="096c1-105">成员</span><span class="sxs-lookup"><span data-stu-id="096c1-105">Member</span></span>|<span data-ttu-id="096c1-106">值</span><span class="sxs-lookup"><span data-stu-id="096c1-106">Value</span></span>|<span data-ttu-id="096c1-107">说明</span><span class="sxs-lookup"><span data-stu-id="096c1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="096c1-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="096c1-108">deviceDefault</span></span>|<span data-ttu-id="096c1-109">0</span><span class="sxs-lookup"><span data-stu-id="096c1-109">{0}</span></span>|<span data-ttu-id="096c1-110">没有由 Intune 配置的值，不要替代用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="096c1-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="096c1-111">none</span><span class="sxs-lookup"><span data-stu-id="096c1-111">none</span></span>|<span data-ttu-id="096c1-112">1</span><span class="sxs-lookup"><span data-stu-id="096c1-112">-1</span></span>|<span data-ttu-id="096c1-113">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="096c1-113">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="096c1-114">尝试</span><span class="sxs-lookup"><span data-stu-id="096c1-114">attempt</span></span>|<span data-ttu-id="096c1-115">2</span><span class="sxs-lookup"><span data-stu-id="096c1-115">-2</span></span>|<span data-ttu-id="096c1-116">尝试 CRL 检查并且检查确认证书后才允许使用证书</span><span class="sxs-lookup"><span data-stu-id="096c1-116">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="096c1-117">require</span><span class="sxs-lookup"><span data-stu-id="096c1-117">Require</span></span>|<span data-ttu-id="096c1-118">3</span><span class="sxs-lookup"><span data-stu-id="096c1-118">-3</span></span>|<span data-ttu-id="096c1-119">允许使用证书之前需要 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="096c1-119">Require a successful CRL check before allowing a certificate</span></span>|








