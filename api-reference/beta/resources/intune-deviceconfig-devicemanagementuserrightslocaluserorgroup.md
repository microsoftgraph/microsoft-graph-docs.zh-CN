---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示用于用户权限设置的本地用户或组的信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68c514635540bcf12db27e8a9ca816573293d3ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174858"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="81020-103">deviceManagementUserRightsLocalUserOrGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="81020-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="81020-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81020-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81020-106">表示用于用户权限设置的本地用户或组的信息。</span><span class="sxs-lookup"><span data-stu-id="81020-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="81020-107">属性</span><span class="sxs-lookup"><span data-stu-id="81020-107">Properties</span></span>
|<span data-ttu-id="81020-108">属性</span><span class="sxs-lookup"><span data-stu-id="81020-108">Property</span></span>|<span data-ttu-id="81020-109">类型</span><span class="sxs-lookup"><span data-stu-id="81020-109">Type</span></span>|<span data-ttu-id="81020-110">说明</span><span class="sxs-lookup"><span data-stu-id="81020-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81020-111">name</span><span class="sxs-lookup"><span data-stu-id="81020-111">name</span></span>|<span data-ttu-id="81020-112">字符串</span><span class="sxs-lookup"><span data-stu-id="81020-112">String</span></span>|<span data-ttu-id="81020-113">此本地用户或组的名称。</span><span class="sxs-lookup"><span data-stu-id="81020-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="81020-114">说明</span><span class="sxs-lookup"><span data-stu-id="81020-114">description</span></span>|<span data-ttu-id="81020-115">字符串</span><span class="sxs-lookup"><span data-stu-id="81020-115">String</span></span>|<span data-ttu-id="81020-116">管理员对此本地用户或组的说明。</span><span class="sxs-lookup"><span data-stu-id="81020-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="81020-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="81020-117">securityIdentifier</span></span>|<span data-ttu-id="81020-118">字符串</span><span class="sxs-lookup"><span data-stu-id="81020-118">String</span></span>|<span data-ttu-id="81020-119">此本地用户或组的安全标识符 (例如 \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="81020-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="81020-120">关系</span><span class="sxs-lookup"><span data-stu-id="81020-120">Relationships</span></span>
<span data-ttu-id="81020-121">无</span><span class="sxs-lookup"><span data-stu-id="81020-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81020-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81020-122">JSON Representation</span></span>
<span data-ttu-id="81020-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81020-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```




