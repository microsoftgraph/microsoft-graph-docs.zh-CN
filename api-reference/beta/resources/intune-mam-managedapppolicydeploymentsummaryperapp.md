---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23966e2017780d3dcfde592d7159576403fe3192
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829748"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="32f64-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="32f64-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="32f64-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32f64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32f64-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32f64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32f64-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="32f64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32f64-107">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="32f64-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="32f64-108">属性</span><span class="sxs-lookup"><span data-stu-id="32f64-108">Properties</span></span>
|<span data-ttu-id="32f64-109">属性</span><span class="sxs-lookup"><span data-stu-id="32f64-109">Property</span></span>|<span data-ttu-id="32f64-110">类型</span><span class="sxs-lookup"><span data-stu-id="32f64-110">Type</span></span>|<span data-ttu-id="32f64-111">说明</span><span class="sxs-lookup"><span data-stu-id="32f64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32f64-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="32f64-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="32f64-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="32f64-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="32f64-114">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="32f64-114">Deployment of an app.</span></span>|
|<span data-ttu-id="32f64-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="32f64-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="32f64-116">Int32</span><span class="sxs-lookup"><span data-stu-id="32f64-116">Int32</span></span>|<span data-ttu-id="32f64-117">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="32f64-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32f64-118">关系</span><span class="sxs-lookup"><span data-stu-id="32f64-118">Relationships</span></span>
<span data-ttu-id="32f64-119">无</span><span class="sxs-lookup"><span data-stu-id="32f64-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="32f64-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32f64-120">JSON Representation</span></span>
<span data-ttu-id="32f64-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32f64-121">Here is a JSON representation of the resource.</span></span>
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





