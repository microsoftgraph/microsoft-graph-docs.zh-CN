---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示用于用户权限设置的本地用户或组的信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdb49ef0b98e3d76d092b1ebf9574d6df8c47d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567198"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="38a50-103">deviceManagementUserRightsLocalUserOrGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="38a50-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="38a50-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38a50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38a50-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38a50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a50-106">表示用于用户权限设置的本地用户或组的信息。</span><span class="sxs-lookup"><span data-stu-id="38a50-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="38a50-107">属性</span><span class="sxs-lookup"><span data-stu-id="38a50-107">Properties</span></span>
|<span data-ttu-id="38a50-108">属性</span><span class="sxs-lookup"><span data-stu-id="38a50-108">Property</span></span>|<span data-ttu-id="38a50-109">类型</span><span class="sxs-lookup"><span data-stu-id="38a50-109">Type</span></span>|<span data-ttu-id="38a50-110">说明</span><span class="sxs-lookup"><span data-stu-id="38a50-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a50-111">name</span><span class="sxs-lookup"><span data-stu-id="38a50-111">name</span></span>|<span data-ttu-id="38a50-112">String</span><span class="sxs-lookup"><span data-stu-id="38a50-112">String</span></span>|<span data-ttu-id="38a50-113">此本地用户或组的名称。</span><span class="sxs-lookup"><span data-stu-id="38a50-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="38a50-114">说明</span><span class="sxs-lookup"><span data-stu-id="38a50-114">description</span></span>|<span data-ttu-id="38a50-115">字符串</span><span class="sxs-lookup"><span data-stu-id="38a50-115">String</span></span>|<span data-ttu-id="38a50-116">管理员对此本地用户或组的说明。</span><span class="sxs-lookup"><span data-stu-id="38a50-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="38a50-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="38a50-117">securityIdentifier</span></span>|<span data-ttu-id="38a50-118">String</span><span class="sxs-lookup"><span data-stu-id="38a50-118">String</span></span>|<span data-ttu-id="38a50-119">此本地用户或组的安全标识符 (例如 \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="38a50-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="38a50-120">关系</span><span class="sxs-lookup"><span data-stu-id="38a50-120">Relationships</span></span>
<span data-ttu-id="38a50-121">无</span><span class="sxs-lookup"><span data-stu-id="38a50-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38a50-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38a50-122">JSON Representation</span></span>
<span data-ttu-id="38a50-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38a50-123">Here is a JSON representation of the resource.</span></span>
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





