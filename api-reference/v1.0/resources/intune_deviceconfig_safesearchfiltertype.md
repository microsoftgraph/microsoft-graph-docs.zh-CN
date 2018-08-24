# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="1423e-101">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1423e-101">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="1423e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1423e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1423e-103">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="1423e-103">Specifies what filter level of safe search is required.</span></span>
## <a name="members"></a><span data-ttu-id="1423e-104">成员</span><span class="sxs-lookup"><span data-stu-id="1423e-104">Members</span></span>
|<span data-ttu-id="1423e-105">成员</span><span class="sxs-lookup"><span data-stu-id="1423e-105">Member</span></span>|<span data-ttu-id="1423e-106">值</span><span class="sxs-lookup"><span data-stu-id="1423e-106">Value</span></span>|<span data-ttu-id="1423e-107">说明</span><span class="sxs-lookup"><span data-stu-id="1423e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1423e-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="1423e-108">UserDefined</span></span>|<span data-ttu-id="1423e-109">0</span><span class="sxs-lookup"><span data-stu-id="1423e-109">{0}</span></span>|<span data-ttu-id="1423e-110">用户自定义，默认值，无特定意图。</span><span class="sxs-lookup"><span data-stu-id="1423e-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="1423e-111">strict</span><span class="sxs-lookup"><span data-stu-id="1423e-111">Strict</span></span>|<span data-ttu-id="1423e-112">1</span><span class="sxs-lookup"><span data-stu-id="1423e-112">-1</span></span>|<span data-ttu-id="1423e-113">严格，针对成人内容的最高级别筛选。</span><span class="sxs-lookup"><span data-stu-id="1423e-113">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="1423e-114">moderate</span><span class="sxs-lookup"><span data-stu-id="1423e-114">Moderate</span></span>|<span data-ttu-id="1423e-115">2</span><span class="sxs-lookup"><span data-stu-id="1423e-115">-2</span></span>|<span data-ttu-id="1423e-116">针对成人内容的中等级别筛选 （有效的搜索结果将不会过滤）。</span><span class="sxs-lookup"><span data-stu-id="1423e-116">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



