---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58aba41699737f0ee76fa7f9aded726d981dec9b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732451"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="d1acb-103">mobileAppTroubleshootingAppTargetHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1acb-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

<span data-ttu-id="d1acb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1acb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1acb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1acb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1acb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1acb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1acb-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="d1acb-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="d1acb-108">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d1acb-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1acb-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1acb-109">Properties</span></span>
|<span data-ttu-id="d1acb-110">属性</span><span class="sxs-lookup"><span data-stu-id="d1acb-110">Property</span></span>|<span data-ttu-id="d1acb-111">类型</span><span class="sxs-lookup"><span data-stu-id="d1acb-111">Type</span></span>|<span data-ttu-id="d1acb-112">说明</span><span class="sxs-lookup"><span data-stu-id="d1acb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1acb-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d1acb-113">occurrenceDateTime</span></span>|<span data-ttu-id="d1acb-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1acb-114">DateTimeOffset</span></span>|<span data-ttu-id="d1acb-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="d1acb-115">Time when the history item occurred.</span></span> <span data-ttu-id="d1acb-116">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d1acb-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d1acb-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d1acb-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="d1acb-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d1acb-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="d1acb-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="d1acb-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="d1acb-120">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d1acb-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d1acb-121">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="d1acb-121">securityGroupId</span></span>|<span data-ttu-id="d1acb-122">String</span><span class="sxs-lookup"><span data-stu-id="d1acb-122">String</span></span>|<span data-ttu-id="d1acb-123">目标为的 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="d1acb-123">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="d1acb-124">runState</span><span class="sxs-lookup"><span data-stu-id="d1acb-124">runState</span></span>|[<span data-ttu-id="d1acb-125">runState</span><span class="sxs-lookup"><span data-stu-id="d1acb-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d1acb-126">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="d1acb-126">Status of the item.</span></span> <span data-ttu-id="d1acb-127">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="d1acb-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="d1acb-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="d1acb-128">errorCode</span></span>|<span data-ttu-id="d1acb-129">String</span><span class="sxs-lookup"><span data-stu-id="d1acb-129">String</span></span>|<span data-ttu-id="d1acb-130">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="d1acb-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1acb-131">关系</span><span class="sxs-lookup"><span data-stu-id="d1acb-131">Relationships</span></span>
<span data-ttu-id="d1acb-132">无</span><span class="sxs-lookup"><span data-stu-id="d1acb-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1acb-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1acb-133">JSON Representation</span></span>
<span data-ttu-id="d1acb-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1acb-134">Here is a JSON representation of the resource.</span></span>
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





