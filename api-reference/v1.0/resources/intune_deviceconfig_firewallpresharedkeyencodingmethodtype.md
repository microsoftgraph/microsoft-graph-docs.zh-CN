# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="32e81-101">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="32e81-101">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="32e81-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="32e81-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32e81-103">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="32e81-103">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="32e81-104">成员</span><span class="sxs-lookup"><span data-stu-id="32e81-104">Members</span></span>
|<span data-ttu-id="32e81-105">成员</span><span class="sxs-lookup"><span data-stu-id="32e81-105">Member</span></span>|<span data-ttu-id="32e81-106">值</span><span class="sxs-lookup"><span data-stu-id="32e81-106">Value</span></span>|<span data-ttu-id="32e81-107">说明</span><span class="sxs-lookup"><span data-stu-id="32e81-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e81-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="32e81-108">deviceDefault</span></span>|<span data-ttu-id="32e81-109">0</span><span class="sxs-lookup"><span data-stu-id="32e81-109">0</span></span>|<span data-ttu-id="32e81-110">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="32e81-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="32e81-111">无</span><span class="sxs-lookup"><span data-stu-id="32e81-111">none</span></span>|<span data-ttu-id="32e81-112">1</span><span class="sxs-lookup"><span data-stu-id="32e81-112">1</span></span>|<span data-ttu-id="32e81-113">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="32e81-113">Preshared key is not encoded.</span></span> <span data-ttu-id="32e81-114">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="32e81-114">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="32e81-115">utF8</span><span class="sxs-lookup"><span data-stu-id="32e81-115">utF8</span></span>|<span data-ttu-id="32e81-116">2</span><span class="sxs-lookup"><span data-stu-id="32e81-116">2</span></span>|<span data-ttu-id="32e81-117">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="32e81-117">Encode the preshared key using UTF-8</span></span>|



