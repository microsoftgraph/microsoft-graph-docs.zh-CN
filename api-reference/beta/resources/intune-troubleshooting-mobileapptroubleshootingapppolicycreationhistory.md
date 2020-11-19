---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb8ef3d71e9e8d80486836f1657df8afc3bc293c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222169"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="cf22d-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf22d-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

<span data-ttu-id="cf22d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf22d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf22d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf22d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf22d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf22d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf22d-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="cf22d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="cf22d-108">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="cf22d-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cf22d-109">属性</span><span class="sxs-lookup"><span data-stu-id="cf22d-109">Properties</span></span>
|<span data-ttu-id="cf22d-110">属性</span><span class="sxs-lookup"><span data-stu-id="cf22d-110">Property</span></span>|<span data-ttu-id="cf22d-111">类型</span><span class="sxs-lookup"><span data-stu-id="cf22d-111">Type</span></span>|<span data-ttu-id="cf22d-112">说明</span><span class="sxs-lookup"><span data-stu-id="cf22d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf22d-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="cf22d-113">occurrenceDateTime</span></span>|<span data-ttu-id="cf22d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf22d-114">DateTimeOffset</span></span>|<span data-ttu-id="cf22d-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="cf22d-115">Time when the history item occurred.</span></span> <span data-ttu-id="cf22d-116">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="cf22d-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="cf22d-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cf22d-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="cf22d-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="cf22d-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="cf22d-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="cf22d-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="cf22d-120">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="cf22d-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="cf22d-121">runState</span><span class="sxs-lookup"><span data-stu-id="cf22d-121">runState</span></span>|[<span data-ttu-id="cf22d-122">runState</span><span class="sxs-lookup"><span data-stu-id="cf22d-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="cf22d-123">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="cf22d-123">Status of the item.</span></span> <span data-ttu-id="cf22d-124">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="cf22d-124">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="cf22d-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="cf22d-125">errorCode</span></span>|<span data-ttu-id="cf22d-126">String</span><span class="sxs-lookup"><span data-stu-id="cf22d-126">String</span></span>|<span data-ttu-id="cf22d-127">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="cf22d-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf22d-128">关系</span><span class="sxs-lookup"><span data-stu-id="cf22d-128">Relationships</span></span>
<span data-ttu-id="cf22d-129">无</span><span class="sxs-lookup"><span data-stu-id="cf22d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf22d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf22d-130">JSON Representation</span></span>
<span data-ttu-id="cf22d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf22d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
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
  "runState": "String",
  "errorCode": "String"
}
```




