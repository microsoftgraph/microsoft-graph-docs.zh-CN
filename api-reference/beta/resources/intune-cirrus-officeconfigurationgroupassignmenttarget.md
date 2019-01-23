---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组工作分配目标。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 411af117999498050288405874bd6b5baff5b6b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422745"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="7524e-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="7524e-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="7524e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7524e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7524e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7524e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7524e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7524e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7524e-107">Office 客户端配置 AAD 组工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="7524e-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="7524e-108">继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7524e-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7524e-109">属性</span><span class="sxs-lookup"><span data-stu-id="7524e-109">Properties</span></span>
|<span data-ttu-id="7524e-110">属性</span><span class="sxs-lookup"><span data-stu-id="7524e-110">Property</span></span>|<span data-ttu-id="7524e-111">类型</span><span class="sxs-lookup"><span data-stu-id="7524e-111">Type</span></span>|<span data-ttu-id="7524e-112">说明</span><span class="sxs-lookup"><span data-stu-id="7524e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7524e-113">groupId</span><span class="sxs-lookup"><span data-stu-id="7524e-113">groupId</span></span>|<span data-ttu-id="7524e-114">String</span><span class="sxs-lookup"><span data-stu-id="7524e-114">String</span></span>|<span data-ttu-id="7524e-115">AAD 组 Id 目标到该设备的配置。</span><span class="sxs-lookup"><span data-stu-id="7524e-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7524e-116">关系</span><span class="sxs-lookup"><span data-stu-id="7524e-116">Relationships</span></span>
<span data-ttu-id="7524e-117">无</span><span class="sxs-lookup"><span data-stu-id="7524e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7524e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7524e-118">JSON Representation</span></span>
<span data-ttu-id="7524e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7524e-119">Here is a JSON representation of the resource.</span></span>
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



