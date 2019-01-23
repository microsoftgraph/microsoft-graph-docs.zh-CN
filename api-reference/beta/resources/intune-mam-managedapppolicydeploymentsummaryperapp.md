---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0e6053a1d690a68359fa30d5e5ac4c0ce5520bc6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411090"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="85bc5-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="85bc5-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="85bc5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="85bc5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85bc5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85bc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85bc5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85bc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85bc5-107">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="85bc5-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="85bc5-108">属性</span><span class="sxs-lookup"><span data-stu-id="85bc5-108">Properties</span></span>
|<span data-ttu-id="85bc5-109">属性</span><span class="sxs-lookup"><span data-stu-id="85bc5-109">Property</span></span>|<span data-ttu-id="85bc5-110">类型</span><span class="sxs-lookup"><span data-stu-id="85bc5-110">Type</span></span>|<span data-ttu-id="85bc5-111">说明</span><span class="sxs-lookup"><span data-stu-id="85bc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85bc5-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="85bc5-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="85bc5-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="85bc5-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="85bc5-114">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="85bc5-114">Deployment of an app.</span></span>|
|<span data-ttu-id="85bc5-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="85bc5-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="85bc5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="85bc5-116">Int32</span></span>|<span data-ttu-id="85bc5-117">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="85bc5-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85bc5-118">关系</span><span class="sxs-lookup"><span data-stu-id="85bc5-118">Relationships</span></span>
<span data-ttu-id="85bc5-119">无</span><span class="sxs-lookup"><span data-stu-id="85bc5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85bc5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85bc5-120">JSON Representation</span></span>
<span data-ttu-id="85bc5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85bc5-121">Here is a JSON representation of the resource.</span></span>
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




