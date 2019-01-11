---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组工作分配目标。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2fe6a668c1f490c167fe61496af14cf2654cebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814768"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="1d447-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d447-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="1d447-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1d447-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d447-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1d447-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d447-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1d447-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d447-107">Office 客户端配置 AAD 组工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="1d447-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="1d447-108">继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1d447-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1d447-109">属性</span><span class="sxs-lookup"><span data-stu-id="1d447-109">Properties</span></span>
|<span data-ttu-id="1d447-110">属性</span><span class="sxs-lookup"><span data-stu-id="1d447-110">Property</span></span>|<span data-ttu-id="1d447-111">类型</span><span class="sxs-lookup"><span data-stu-id="1d447-111">Type</span></span>|<span data-ttu-id="1d447-112">说明</span><span class="sxs-lookup"><span data-stu-id="1d447-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d447-113">groupId</span><span class="sxs-lookup"><span data-stu-id="1d447-113">groupId</span></span>|<span data-ttu-id="1d447-114">字符串</span><span class="sxs-lookup"><span data-stu-id="1d447-114">String</span></span>|<span data-ttu-id="1d447-115">AAD 组 Id 目标到该设备的配置。</span><span class="sxs-lookup"><span data-stu-id="1d447-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d447-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="1d447-116">Relationships</span></span>
<span data-ttu-id="1d447-117">无</span><span class="sxs-lookup"><span data-stu-id="1d447-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d447-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d447-118">JSON Representation</span></span>
<span data-ttu-id="1d447-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d447-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



