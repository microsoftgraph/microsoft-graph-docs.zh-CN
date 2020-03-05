---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf9ff99bdcbfb7ea484a656c540449161a53d45d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448359"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="dac3f-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="dac3f-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="dac3f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dac3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dac3f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dac3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dac3f-106">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="dac3f-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="dac3f-107">属性</span><span class="sxs-lookup"><span data-stu-id="dac3f-107">Properties</span></span>
|<span data-ttu-id="dac3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="dac3f-108">Property</span></span>|<span data-ttu-id="dac3f-109">类型</span><span class="sxs-lookup"><span data-stu-id="dac3f-109">Type</span></span>|<span data-ttu-id="dac3f-110">说明</span><span class="sxs-lookup"><span data-stu-id="dac3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dac3f-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="dac3f-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="dac3f-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="dac3f-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="dac3f-113">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="dac3f-113">Deployment of an app.</span></span>|
|<span data-ttu-id="dac3f-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="dac3f-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="dac3f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="dac3f-115">Int32</span></span>|<span data-ttu-id="dac3f-116">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="dac3f-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dac3f-117">关系</span><span class="sxs-lookup"><span data-stu-id="dac3f-117">Relationships</span></span>
<span data-ttu-id="dac3f-118">无</span><span class="sxs-lookup"><span data-stu-id="dac3f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dac3f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dac3f-119">JSON Representation</span></span>
<span data-ttu-id="dac3f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dac3f-120">Here is a JSON representation of the resource.</span></span>
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




