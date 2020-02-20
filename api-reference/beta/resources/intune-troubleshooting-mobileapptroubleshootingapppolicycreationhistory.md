---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0d83f07cfa71c84cb0db99b7ea6e26822177f8f
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159078"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="4bb5c-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bb5c-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="4bb5c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bb5c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bb5c-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="4bb5c-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bb5c-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4bb5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bb5c-108">Properties</span></span>
|<span data-ttu-id="4bb5c-109">属性</span><span class="sxs-lookup"><span data-stu-id="4bb5c-109">Property</span></span>|<span data-ttu-id="4bb5c-110">类型</span><span class="sxs-lookup"><span data-stu-id="4bb5c-110">Type</span></span>|<span data-ttu-id="4bb5c-111">说明</span><span class="sxs-lookup"><span data-stu-id="4bb5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb5c-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb5c-112">occurrenceDateTime</span></span>|<span data-ttu-id="4bb5c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb5c-113">DateTimeOffset</span></span>|<span data-ttu-id="4bb5c-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-114">Time when the history item occurred.</span></span> <span data-ttu-id="4bb5c-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bb5c-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="4bb5c-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4bb5c-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="4bb5c-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4bb5c-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="4bb5c-118">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="4bb5c-119">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4bb5c-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="4bb5c-120">runState</span><span class="sxs-lookup"><span data-stu-id="4bb5c-120">runState</span></span>|[<span data-ttu-id="4bb5c-121">runState</span><span class="sxs-lookup"><span data-stu-id="4bb5c-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4bb5c-122">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-122">Status of the item.</span></span> <span data-ttu-id="4bb5c-123">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-123">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="4bb5c-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="4bb5c-124">errorCode</span></span>|<span data-ttu-id="4bb5c-125">String</span><span class="sxs-lookup"><span data-stu-id="4bb5c-125">String</span></span>|<span data-ttu-id="4bb5c-126">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bb5c-127">关系</span><span class="sxs-lookup"><span data-stu-id="4bb5c-127">Relationships</span></span>
<span data-ttu-id="4bb5c-128">无</span><span class="sxs-lookup"><span data-stu-id="4bb5c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bb5c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bb5c-129">JSON Representation</span></span>
<span data-ttu-id="4bb5c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bb5c-130">Here is a JSON representation of the resource.</span></span>
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



