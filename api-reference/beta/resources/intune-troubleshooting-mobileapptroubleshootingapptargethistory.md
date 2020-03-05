---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 074be97a5090b64afc8fee6dd61203285702d896
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523301"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="e1aff-103">mobileAppTroubleshootingAppTargetHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1aff-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

<span data-ttu-id="e1aff-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e1aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1aff-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1aff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1aff-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="e1aff-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e1aff-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e1aff-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1aff-109">属性</span><span class="sxs-lookup"><span data-stu-id="e1aff-109">Properties</span></span>
|<span data-ttu-id="e1aff-110">属性</span><span class="sxs-lookup"><span data-stu-id="e1aff-110">Property</span></span>|<span data-ttu-id="e1aff-111">类型</span><span class="sxs-lookup"><span data-stu-id="e1aff-111">Type</span></span>|<span data-ttu-id="e1aff-112">说明</span><span class="sxs-lookup"><span data-stu-id="e1aff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1aff-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e1aff-113">occurrenceDateTime</span></span>|<span data-ttu-id="e1aff-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1aff-114">DateTimeOffset</span></span>|<span data-ttu-id="e1aff-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e1aff-115">Time when the history item occurred.</span></span> <span data-ttu-id="e1aff-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e1aff-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e1aff-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e1aff-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e1aff-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e1aff-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e1aff-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="e1aff-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="e1aff-120">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e1aff-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e1aff-121">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="e1aff-121">securityGroupId</span></span>|<span data-ttu-id="e1aff-122">String</span><span class="sxs-lookup"><span data-stu-id="e1aff-122">String</span></span>|<span data-ttu-id="e1aff-123">目标为的 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="e1aff-123">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="e1aff-124">runState</span><span class="sxs-lookup"><span data-stu-id="e1aff-124">runState</span></span>|[<span data-ttu-id="e1aff-125">runState</span><span class="sxs-lookup"><span data-stu-id="e1aff-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e1aff-126">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="e1aff-126">Status of the item.</span></span> <span data-ttu-id="e1aff-127">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="e1aff-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="e1aff-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="e1aff-128">errorCode</span></span>|<span data-ttu-id="e1aff-129">String</span><span class="sxs-lookup"><span data-stu-id="e1aff-129">String</span></span>|<span data-ttu-id="e1aff-130">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="e1aff-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1aff-131">关系</span><span class="sxs-lookup"><span data-stu-id="e1aff-131">Relationships</span></span>
<span data-ttu-id="e1aff-132">无</span><span class="sxs-lookup"><span data-stu-id="e1aff-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1aff-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1aff-133">JSON Representation</span></span>
<span data-ttu-id="e1aff-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1aff-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```



