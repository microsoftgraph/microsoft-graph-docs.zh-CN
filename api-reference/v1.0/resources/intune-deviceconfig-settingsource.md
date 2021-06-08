---
title: settingSource 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2cfe802c344550fa15c84614911db55493e93125
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759971"
---
# <a name="settingsource-resource-type"></a><span data-ttu-id="12d02-103">settingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="12d02-103">settingSource resource type</span></span>

<span data-ttu-id="12d02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12d02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12d02-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12d02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d02-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12d02-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="12d02-107">属性</span><span class="sxs-lookup"><span data-stu-id="12d02-107">Properties</span></span>
|<span data-ttu-id="12d02-108">属性</span><span class="sxs-lookup"><span data-stu-id="12d02-108">Property</span></span>|<span data-ttu-id="12d02-109">类型</span><span class="sxs-lookup"><span data-stu-id="12d02-109">Type</span></span>|<span data-ttu-id="12d02-110">说明</span><span class="sxs-lookup"><span data-stu-id="12d02-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d02-111">id</span><span class="sxs-lookup"><span data-stu-id="12d02-111">id</span></span>|<span data-ttu-id="12d02-112">String</span><span class="sxs-lookup"><span data-stu-id="12d02-112">String</span></span>|<span data-ttu-id="12d02-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12d02-113">Not yet documented</span></span>|
|<span data-ttu-id="12d02-114">displayName</span><span class="sxs-lookup"><span data-stu-id="12d02-114">displayName</span></span>|<span data-ttu-id="12d02-115">String</span><span class="sxs-lookup"><span data-stu-id="12d02-115">String</span></span>|<span data-ttu-id="12d02-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12d02-116">Not yet documented</span></span>|
|<span data-ttu-id="12d02-117">sourceType</span><span class="sxs-lookup"><span data-stu-id="12d02-117">sourceType</span></span>|[<span data-ttu-id="12d02-118">settingSourceType</span><span class="sxs-lookup"><span data-stu-id="12d02-118">settingSourceType</span></span>](../resources/intune-deviceconfig-settingsourcetype.md)|<span data-ttu-id="12d02-119">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="12d02-119">Not yet documented.</span></span> <span data-ttu-id="12d02-120">可取值为：`deviceConfiguration`、`deviceIntent`。</span><span class="sxs-lookup"><span data-stu-id="12d02-120">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12d02-121">关系</span><span class="sxs-lookup"><span data-stu-id="12d02-121">Relationships</span></span>
<span data-ttu-id="12d02-122">无</span><span class="sxs-lookup"><span data-stu-id="12d02-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12d02-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12d02-123">JSON Representation</span></span>
<span data-ttu-id="12d02-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12d02-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.settingSource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingSource",
  "id": "String (identifier)",
  "displayName": "String",
  "sourceType": "String"
}
```




