# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="0b87c-101">applePushNotificationCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b87c-101">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="0b87c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b87c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b87c-103">Apple 推送通知证书。</span><span class="sxs-lookup"><span data-stu-id="0b87c-103">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="0b87c-104">方法</span><span class="sxs-lookup"><span data-stu-id="0b87c-104">Methods</span></span>
|<span data-ttu-id="0b87c-105">方法</span><span class="sxs-lookup"><span data-stu-id="0b87c-105">Method</span></span>|<span data-ttu-id="0b87c-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b87c-106">Return Type</span></span>|<span data-ttu-id="0b87c-107">说明</span><span class="sxs-lookup"><span data-stu-id="0b87c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b87c-108">获取 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0b87c-108">Get applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_get.md)|[<span data-ttu-id="0b87c-109">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0b87c-109">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="0b87c-110">读取 [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b87c-110">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="0b87c-111">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0b87c-111">Update applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_update.md)|[<span data-ttu-id="0b87c-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0b87c-112">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="0b87c-113">更新 [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b87c-113">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="0b87c-114">downloadApplePushNotificationCertificateSigningRequest 函数</span><span class="sxs-lookup"><span data-stu-id="0b87c-114">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="0b87c-115">String</span><span class="sxs-lookup"><span data-stu-id="0b87c-115">String</span></span>|<span data-ttu-id="0b87c-116">下载 Apple 推送通知证书签名请求</span><span class="sxs-lookup"><span data-stu-id="0b87c-116">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="0b87c-117">属性</span><span class="sxs-lookup"><span data-stu-id="0b87c-117">Properties</span></span>
|<span data-ttu-id="0b87c-118">属性</span><span class="sxs-lookup"><span data-stu-id="0b87c-118">Property</span></span>|<span data-ttu-id="0b87c-119">类型</span><span class="sxs-lookup"><span data-stu-id="0b87c-119">Type</span></span>|<span data-ttu-id="0b87c-120">说明</span><span class="sxs-lookup"><span data-stu-id="0b87c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b87c-121">id</span><span class="sxs-lookup"><span data-stu-id="0b87c-121">id</span></span>|<span data-ttu-id="0b87c-122">String</span><span class="sxs-lookup"><span data-stu-id="0b87c-122">String</span></span>|<span data-ttu-id="0b87c-123">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="0b87c-123">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="0b87c-124">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="0b87c-124">appleIdentifier</span></span>|<span data-ttu-id="0b87c-125">String</span><span class="sxs-lookup"><span data-stu-id="0b87c-125">String</span></span>|<span data-ttu-id="0b87c-126">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="0b87c-126">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="0b87c-127">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="0b87c-127">topicIdentifier</span></span>|<span data-ttu-id="0b87c-128">String</span><span class="sxs-lookup"><span data-stu-id="0b87c-128">String</span></span>|<span data-ttu-id="0b87c-129">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="0b87c-129">Topic Id.</span></span>|
|<span data-ttu-id="0b87c-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b87c-130">lastModifiedDateTime</span></span>|<span data-ttu-id="0b87c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b87c-131">DateTimeOffset</span></span>|<span data-ttu-id="0b87c-132">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b87c-132">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="0b87c-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b87c-133">expirationDateTime</span></span>|<span data-ttu-id="0b87c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b87c-134">DateTimeOffset</span></span>|<span data-ttu-id="0b87c-135">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b87c-135">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="0b87c-136">certificate</span><span class="sxs-lookup"><span data-stu-id="0b87c-136">certificate</span></span>|<span data-ttu-id="0b87c-137">String</span><span class="sxs-lookup"><span data-stu-id="0b87c-137">String</span></span>|<span data-ttu-id="0b87c-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0b87c-138">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b87c-139">关系</span><span class="sxs-lookup"><span data-stu-id="0b87c-139">Relationships</span></span>
<span data-ttu-id="0b87c-140">无</span><span class="sxs-lookup"><span data-stu-id="0b87c-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b87c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b87c-141">JSON Representation</span></span>
<span data-ttu-id="0b87c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b87c-142">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



