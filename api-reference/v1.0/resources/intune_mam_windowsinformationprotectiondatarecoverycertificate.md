# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="1c338-101">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c338-101">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="1c338-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c338-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c338-103">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1c338-103">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="1c338-104">属性</span><span class="sxs-lookup"><span data-stu-id="1c338-104">Properties</span></span>
|<span data-ttu-id="1c338-105">属性</span><span class="sxs-lookup"><span data-stu-id="1c338-105">Property</span></span>|<span data-ttu-id="1c338-106">类型</span><span class="sxs-lookup"><span data-stu-id="1c338-106">Type</span></span>|<span data-ttu-id="1c338-107">说明</span><span class="sxs-lookup"><span data-stu-id="1c338-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c338-108">SubjectName</span><span class="sxs-lookup"><span data-stu-id="1c338-108">subjectName</span></span>|<span data-ttu-id="1c338-109">String</span><span class="sxs-lookup"><span data-stu-id="1c338-109">String</span></span>|<span data-ttu-id="1c338-110">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="1c338-110">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="1c338-111">description</span><span class="sxs-lookup"><span data-stu-id="1c338-111">description</span></span>|<span data-ttu-id="1c338-112">String</span><span class="sxs-lookup"><span data-stu-id="1c338-112">String</span></span>|<span data-ttu-id="1c338-113">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="1c338-113">Data recovery Certificate description</span></span>|
|<span data-ttu-id="1c338-114">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1c338-114">expirationDateTime</span></span>|<span data-ttu-id="1c338-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c338-115">DateTimeOffset</span></span>|<span data-ttu-id="1c338-116">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="1c338-116">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="1c338-117">证书</span><span class="sxs-lookup"><span data-stu-id="1c338-117">certificate</span></span>|<span data-ttu-id="1c338-118">Binary</span><span class="sxs-lookup"><span data-stu-id="1c338-118">Binary</span></span>|<span data-ttu-id="1c338-119">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="1c338-119">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c338-120">关系</span><span class="sxs-lookup"><span data-stu-id="1c338-120">Relationships</span></span>
<span data-ttu-id="1c338-121">无</span><span class="sxs-lookup"><span data-stu-id="1c338-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c338-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c338-122">JSON Representation</span></span>
<span data-ttu-id="1c338-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c338-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```








