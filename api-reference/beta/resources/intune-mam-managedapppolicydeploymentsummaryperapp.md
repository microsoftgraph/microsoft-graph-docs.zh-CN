---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
ms.openlocfilehash: 2555fd72bb5b7b3e4018d99a7ddbdd6627b2cef3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046304"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="99185-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="99185-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="99185-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99185-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99185-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99185-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99185-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99185-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99185-107">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="99185-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="99185-108">属性</span><span class="sxs-lookup"><span data-stu-id="99185-108">Properties</span></span>
|<span data-ttu-id="99185-109">属性</span><span class="sxs-lookup"><span data-stu-id="99185-109">Property</span></span>|<span data-ttu-id="99185-110">类型</span><span class="sxs-lookup"><span data-stu-id="99185-110">Type</span></span>|<span data-ttu-id="99185-111">说明</span><span class="sxs-lookup"><span data-stu-id="99185-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99185-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="99185-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="99185-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="99185-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="99185-114">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="99185-114">Deployment of an app.</span></span>|
|<span data-ttu-id="99185-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="99185-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="99185-116">Int32</span><span class="sxs-lookup"><span data-stu-id="99185-116">Int32</span></span>|<span data-ttu-id="99185-117">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="99185-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99185-118">关系</span><span class="sxs-lookup"><span data-stu-id="99185-118">Relationships</span></span>
<span data-ttu-id="99185-119">无</span><span class="sxs-lookup"><span data-stu-id="99185-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99185-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99185-120">JSON Representation</span></span>
<span data-ttu-id="99185-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99185-121">Here is a JSON representation of the resource.</span></span>
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





