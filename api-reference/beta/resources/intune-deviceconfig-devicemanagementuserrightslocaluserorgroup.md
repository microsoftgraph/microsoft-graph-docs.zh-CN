---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示用于用户权限设置的本地用户或组的信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d288e1f8936c7f1246b0e66eebeaefc910dadc00
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283404"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="ad406-103">deviceManagementUserRightsLocalUserOrGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad406-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="ad406-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad406-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad406-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ad406-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad406-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad406-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad406-107">表示用于用户权限设置的本地用户或组的信息。</span><span class="sxs-lookup"><span data-stu-id="ad406-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="ad406-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad406-108">Properties</span></span>
|<span data-ttu-id="ad406-109">属性</span><span class="sxs-lookup"><span data-stu-id="ad406-109">Property</span></span>|<span data-ttu-id="ad406-110">类型</span><span class="sxs-lookup"><span data-stu-id="ad406-110">Type</span></span>|<span data-ttu-id="ad406-111">Description</span><span class="sxs-lookup"><span data-stu-id="ad406-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad406-112">name</span><span class="sxs-lookup"><span data-stu-id="ad406-112">name</span></span>|<span data-ttu-id="ad406-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ad406-113">String</span></span>|<span data-ttu-id="ad406-114">此本地用户或组的名称。</span><span class="sxs-lookup"><span data-stu-id="ad406-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="ad406-115">description</span><span class="sxs-lookup"><span data-stu-id="ad406-115">description</span></span>|<span data-ttu-id="ad406-116">字符串</span><span class="sxs-lookup"><span data-stu-id="ad406-116">String</span></span>|<span data-ttu-id="ad406-117">管理员对此本地用户或组的说明。</span><span class="sxs-lookup"><span data-stu-id="ad406-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="ad406-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="ad406-118">securityIdentifier</span></span>|<span data-ttu-id="ad406-119">字符串</span><span class="sxs-lookup"><span data-stu-id="ad406-119">String</span></span>|<span data-ttu-id="ad406-120">此本地用户或组的安全标识符 (例如 \* S-1-5-32-544) 。</span><span class="sxs-lookup"><span data-stu-id="ad406-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad406-121">关系</span><span class="sxs-lookup"><span data-stu-id="ad406-121">Relationships</span></span>
<span data-ttu-id="ad406-122">无</span><span class="sxs-lookup"><span data-stu-id="ad406-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad406-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad406-123">JSON Representation</span></span>
<span data-ttu-id="ad406-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad406-124">Here is a JSON representation of the resource.</span></span>
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




