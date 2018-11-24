# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="51221-101">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="51221-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="51221-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="51221-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51221-103">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="51221-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="51221-104">属性</span><span class="sxs-lookup"><span data-stu-id="51221-104">Properties</span></span>
|<span data-ttu-id="51221-105">属性</span><span class="sxs-lookup"><span data-stu-id="51221-105">Property</span></span>|<span data-ttu-id="51221-106">类型</span><span class="sxs-lookup"><span data-stu-id="51221-106">Type</span></span>|<span data-ttu-id="51221-107">说明</span><span class="sxs-lookup"><span data-stu-id="51221-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51221-108">bundleID</span><span class="sxs-lookup"><span data-stu-id="51221-108">bundleID</span></span>|<span data-ttu-id="51221-109">String</span><span class="sxs-lookup"><span data-stu-id="51221-109">String</span></span>|<span data-ttu-id="51221-110">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="51221-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="51221-111">appName</span><span class="sxs-lookup"><span data-stu-id="51221-111">appName</span></span>|<span data-ttu-id="51221-112">String</span><span class="sxs-lookup"><span data-stu-id="51221-112">String</span></span>|<span data-ttu-id="51221-113">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="51221-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="51221-114">发布者</span><span class="sxs-lookup"><span data-stu-id="51221-114">publisher</span></span>|<span data-ttu-id="51221-115">String</span><span class="sxs-lookup"><span data-stu-id="51221-115">String</span></span>|<span data-ttu-id="51221-116">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="51221-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="51221-117">enabled</span><span class="sxs-lookup"><span data-stu-id="51221-117">enabled</span></span>|<span data-ttu-id="51221-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="51221-118">Boolean</span></span>|<span data-ttu-id="51221-119">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="51221-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="51221-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="51221-120">showInNotificationCenter</span></span>|<span data-ttu-id="51221-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="51221-121">Boolean</span></span>|<span data-ttu-id="51221-122">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="51221-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="51221-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="51221-123">showOnLockScreen</span></span>|<span data-ttu-id="51221-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="51221-124">Boolean</span></span>|<span data-ttu-id="51221-125">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="51221-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="51221-126">alertType</span><span class="sxs-lookup"><span data-stu-id="51221-126">alertType</span></span>|[<span data-ttu-id="51221-127">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="51221-127">iosNotificationAlertType</span></span>](../resources/intune_deviceconfig_iosnotificationalerttype.md)|<span data-ttu-id="51221-128">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="51221-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="51221-129">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="51221-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="51221-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="51221-130">badgesEnabled</span></span>|<span data-ttu-id="51221-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="51221-131">Boolean</span></span>|<span data-ttu-id="51221-132">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="51221-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="51221-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="51221-133">soundsEnabled</span></span>|<span data-ttu-id="51221-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="51221-134">Boolean</span></span>|<span data-ttu-id="51221-135">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="51221-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51221-136">关系</span><span class="sxs-lookup"><span data-stu-id="51221-136">Relationships</span></span>
<span data-ttu-id="51221-137">无</span><span class="sxs-lookup"><span data-stu-id="51221-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51221-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51221-138">JSON Representation</span></span>
<span data-ttu-id="51221-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51221-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



