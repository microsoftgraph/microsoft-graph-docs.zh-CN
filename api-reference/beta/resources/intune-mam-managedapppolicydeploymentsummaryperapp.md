---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d17dfb7cc288edb37f82587dfe76b65ebe15efd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781577"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="9b341-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b341-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="9b341-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b341-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b341-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b341-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b341-106">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="9b341-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="9b341-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b341-107">Properties</span></span>
|<span data-ttu-id="9b341-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b341-108">Property</span></span>|<span data-ttu-id="9b341-109">类型</span><span class="sxs-lookup"><span data-stu-id="9b341-109">Type</span></span>|<span data-ttu-id="9b341-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b341-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b341-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9b341-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="9b341-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9b341-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9b341-113">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="9b341-113">Deployment of an app.</span></span>|
|<span data-ttu-id="9b341-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="9b341-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="9b341-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9b341-115">Int32</span></span>|<span data-ttu-id="9b341-116">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9b341-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b341-117">关系</span><span class="sxs-lookup"><span data-stu-id="9b341-117">Relationships</span></span>
<span data-ttu-id="9b341-118">无</span><span class="sxs-lookup"><span data-stu-id="9b341-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b341-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b341-119">JSON Representation</span></span>
<span data-ttu-id="9b341-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b341-120">Here is a JSON representation of the resource.</span></span>
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



