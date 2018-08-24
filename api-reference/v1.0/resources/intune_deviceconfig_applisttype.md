# <a name="applisttype-enum-type"></a><span data-ttu-id="c00a0-101">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c00a0-101">appListType enum type</span></span>

> <span data-ttu-id="c00a0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c00a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c00a0-103">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="c00a0-103">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="c00a0-104">成员</span><span class="sxs-lookup"><span data-stu-id="c00a0-104">Members</span></span>
|<span data-ttu-id="c00a0-105">成员</span><span class="sxs-lookup"><span data-stu-id="c00a0-105">Member</span></span>|<span data-ttu-id="c00a0-106">值</span><span class="sxs-lookup"><span data-stu-id="c00a0-106">Value</span></span>|<span data-ttu-id="c00a0-107">说明</span><span class="sxs-lookup"><span data-stu-id="c00a0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c00a0-108">none</span><span class="sxs-lookup"><span data-stu-id="c00a0-108">none</span></span>|<span data-ttu-id="c00a0-109">0</span><span class="sxs-lookup"><span data-stu-id="c00a0-109">{0}</span></span>|<span data-ttu-id="c00a0-110">默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="c00a0-110">Default value, no intent.</span></span>|
|<span data-ttu-id="c00a0-111">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c00a0-111">appsInListCompliant</span></span>|<span data-ttu-id="c00a0-112">1</span><span class="sxs-lookup"><span data-stu-id="c00a0-112">-1</span></span>|<span data-ttu-id="c00a0-113">列表代表将被视为合规的应用程序 （仅在列表上的应用程序视为合规）。</span><span class="sxs-lookup"><span data-stu-id="c00a0-113">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="c00a0-114">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c00a0-114">appsNotInListCompliant</span></span>|<span data-ttu-id="c00a0-115">2</span><span class="sxs-lookup"><span data-stu-id="c00a0-115">-2</span></span>|<span data-ttu-id="c00a0-116">列表代表将被视为不合规的应用程序 （所有应用程序都合规，列表上的应用程序除外）。</span><span class="sxs-lookup"><span data-stu-id="c00a0-116">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



