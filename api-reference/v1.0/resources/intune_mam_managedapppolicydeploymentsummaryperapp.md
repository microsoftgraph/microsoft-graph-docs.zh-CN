# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="9e8fd-101">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e8fd-101">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="9e8fd-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e8fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e8fd-103">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="9e8fd-103">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="9e8fd-104">属性</span><span class="sxs-lookup"><span data-stu-id="9e8fd-104">Properties</span></span>
|<span data-ttu-id="9e8fd-105">属性</span><span class="sxs-lookup"><span data-stu-id="9e8fd-105">Property</span></span>|<span data-ttu-id="9e8fd-106">类型</span><span class="sxs-lookup"><span data-stu-id="9e8fd-106">Type</span></span>|<span data-ttu-id="9e8fd-107">说明</span><span class="sxs-lookup"><span data-stu-id="9e8fd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e8fd-108">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e8fd-108">mobileAppIdentifier</span></span>|[<span data-ttu-id="9e8fd-109">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e8fd-109">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="9e8fd-110">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="9e8fd-110">Deployment of an app.</span></span>|
|<span data-ttu-id="9e8fd-111">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="9e8fd-111">configurationAppliedUserCount</span></span>|<span data-ttu-id="9e8fd-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9e8fd-112">Int32</span></span>|<span data-ttu-id="9e8fd-113">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9e8fd-113">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e8fd-114">关系</span><span class="sxs-lookup"><span data-stu-id="9e8fd-114">Relationships</span></span>
<span data-ttu-id="9e8fd-115">无</span><span class="sxs-lookup"><span data-stu-id="9e8fd-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e8fd-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e8fd-116">JSON Representation</span></span>
<span data-ttu-id="9e8fd-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e8fd-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



