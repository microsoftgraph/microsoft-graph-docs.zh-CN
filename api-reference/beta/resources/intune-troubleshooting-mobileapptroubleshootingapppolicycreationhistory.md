---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbbf575c7eaecb93e0256d6f672d0c4d6bdd0edf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570038"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="39f51-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="39f51-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="39f51-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="39f51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39f51-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39f51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39f51-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="39f51-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="39f51-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="39f51-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="39f51-108">属性</span><span class="sxs-lookup"><span data-stu-id="39f51-108">Properties</span></span>
|<span data-ttu-id="39f51-109">属性</span><span class="sxs-lookup"><span data-stu-id="39f51-109">Property</span></span>|<span data-ttu-id="39f51-110">类型</span><span class="sxs-lookup"><span data-stu-id="39f51-110">Type</span></span>|<span data-ttu-id="39f51-111">说明</span><span class="sxs-lookup"><span data-stu-id="39f51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f51-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="39f51-112">occurrenceDateTime</span></span>|<span data-ttu-id="39f51-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39f51-113">DateTimeOffset</span></span>|<span data-ttu-id="39f51-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="39f51-114">Time when the history item occurred.</span></span> <span data-ttu-id="39f51-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="39f51-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="39f51-116">runState</span><span class="sxs-lookup"><span data-stu-id="39f51-116">runState</span></span>|[<span data-ttu-id="39f51-117">runState</span><span class="sxs-lookup"><span data-stu-id="39f51-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="39f51-118">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="39f51-118">Status of the item.</span></span> <span data-ttu-id="39f51-119">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="39f51-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="39f51-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="39f51-120">errorCode</span></span>|<span data-ttu-id="39f51-121">String</span><span class="sxs-lookup"><span data-stu-id="39f51-121">String</span></span>|<span data-ttu-id="39f51-122">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="39f51-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39f51-123">关系</span><span class="sxs-lookup"><span data-stu-id="39f51-123">Relationships</span></span>
<span data-ttu-id="39f51-124">无</span><span class="sxs-lookup"><span data-stu-id="39f51-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39f51-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39f51-125">JSON Representation</span></span>
<span data-ttu-id="39f51-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39f51-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```



