# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="08656-101">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="08656-101">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="08656-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="08656-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08656-103">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="08656-103">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="08656-104">属性</span><span class="sxs-lookup"><span data-stu-id="08656-104">Properties</span></span>
|<span data-ttu-id="08656-105">属性</span><span class="sxs-lookup"><span data-stu-id="08656-105">Property</span></span>|<span data-ttu-id="08656-106">类型</span><span class="sxs-lookup"><span data-stu-id="08656-106">Type</span></span>|<span data-ttu-id="08656-107">说明</span><span class="sxs-lookup"><span data-stu-id="08656-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08656-108">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="08656-108">mobileAppIdentifier</span></span>|[<span data-ttu-id="08656-109">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="08656-109">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="08656-110">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="08656-110">Deployment of an app.</span></span>|
|<span data-ttu-id="08656-111">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="08656-111">configurationAppliedUserCount</span></span>|<span data-ttu-id="08656-112">Int32</span><span class="sxs-lookup"><span data-stu-id="08656-112">Int32</span></span>|<span data-ttu-id="08656-113">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="08656-113">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08656-114">关系</span><span class="sxs-lookup"><span data-stu-id="08656-114">Relationships</span></span>
<span data-ttu-id="08656-115">无</span><span class="sxs-lookup"><span data-stu-id="08656-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08656-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08656-116">JSON Representation</span></span>
<span data-ttu-id="08656-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08656-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```



