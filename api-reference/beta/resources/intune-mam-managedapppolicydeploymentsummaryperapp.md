---
title: managedAppPolicyDeploymentSummaryPerApp 资源类型
description: 表示每个应用的策略部署摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1174e46f40a7f80944cf686a403edb0db60cb1fd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994725"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="39b93-103">managedAppPolicyDeploymentSummaryPerApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="39b93-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="39b93-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="39b93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39b93-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39b93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39b93-106">表示每个应用的策略部署摘要。</span><span class="sxs-lookup"><span data-stu-id="39b93-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="39b93-107">属性</span><span class="sxs-lookup"><span data-stu-id="39b93-107">Properties</span></span>
|<span data-ttu-id="39b93-108">属性</span><span class="sxs-lookup"><span data-stu-id="39b93-108">Property</span></span>|<span data-ttu-id="39b93-109">类型</span><span class="sxs-lookup"><span data-stu-id="39b93-109">Type</span></span>|<span data-ttu-id="39b93-110">说明</span><span class="sxs-lookup"><span data-stu-id="39b93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39b93-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="39b93-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="39b93-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="39b93-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="39b93-113">应用的部署。</span><span class="sxs-lookup"><span data-stu-id="39b93-113">Deployment of an app.</span></span>|
|<span data-ttu-id="39b93-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="39b93-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="39b93-115">Int32</span><span class="sxs-lookup"><span data-stu-id="39b93-115">Int32</span></span>|<span data-ttu-id="39b93-116">应用策略的用户数量。</span><span class="sxs-lookup"><span data-stu-id="39b93-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39b93-117">关系</span><span class="sxs-lookup"><span data-stu-id="39b93-117">Relationships</span></span>
<span data-ttu-id="39b93-118">无</span><span class="sxs-lookup"><span data-stu-id="39b93-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39b93-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39b93-119">JSON Representation</span></span>
<span data-ttu-id="39b93-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39b93-120">Here is a JSON representation of the resource.</span></span>
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





