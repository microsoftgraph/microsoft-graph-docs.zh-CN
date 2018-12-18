---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: tfitzmac
ms.openlocfilehash: 95c05696f6c080f90b9de61c309a577924e599b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354339"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="9e397-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e397-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="9e397-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e397-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e397-105">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="9e397-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="9e397-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e397-106">Properties</span></span>
|<span data-ttu-id="9e397-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e397-107">Property</span></span>|<span data-ttu-id="9e397-108">类型</span><span class="sxs-lookup"><span data-stu-id="9e397-108">Type</span></span>|<span data-ttu-id="9e397-109">说明</span><span class="sxs-lookup"><span data-stu-id="9e397-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e397-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e397-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="9e397-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e397-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9e397-112">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="9e397-112">Deployment of an app.</span></span>|
|<span data-ttu-id="9e397-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="9e397-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="9e397-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9e397-114">Int32</span></span>|<span data-ttu-id="9e397-115">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9e397-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e397-116">关系</span><span class="sxs-lookup"><span data-stu-id="9e397-116">Relationships</span></span>
<span data-ttu-id="9e397-117">无</span><span class="sxs-lookup"><span data-stu-id="9e397-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e397-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e397-118">JSON Representation</span></span>
<span data-ttu-id="9e397-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e397-119">Here is a JSON representation of the resource.</span></span>
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



