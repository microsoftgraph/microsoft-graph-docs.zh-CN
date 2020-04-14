---
title: companyPortalBlockedAction 资源类型
description: 按平台和设备所有权类型对公司门户的阻止的操作
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3ebaea7b233a4a596db12e93643992d6ef7a15cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457377"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="a544e-103">companyPortalBlockedAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a544e-103">companyPortalBlockedAction resource type</span></span>

<span data-ttu-id="a544e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a544e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a544e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a544e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a544e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a544e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a544e-107">按平台和设备所有权类型对公司门户的阻止的操作</span><span class="sxs-lookup"><span data-stu-id="a544e-107">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="a544e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a544e-108">Properties</span></span>
|<span data-ttu-id="a544e-109">属性</span><span class="sxs-lookup"><span data-stu-id="a544e-109">Property</span></span>|<span data-ttu-id="a544e-110">类型</span><span class="sxs-lookup"><span data-stu-id="a544e-110">Type</span></span>|<span data-ttu-id="a544e-111">说明</span><span class="sxs-lookup"><span data-stu-id="a544e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a544e-112">platform</span><span class="sxs-lookup"><span data-stu-id="a544e-112">platform</span></span>|[<span data-ttu-id="a544e-113">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="a544e-113">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="a544e-114">设备 OS/平台。</span><span class="sxs-lookup"><span data-stu-id="a544e-114">Device OS/Platform.</span></span> <span data-ttu-id="a544e-115">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="a544e-115">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="a544e-116">所有者</span><span class="sxs-lookup"><span data-stu-id="a544e-116">ownerType</span></span>|[<span data-ttu-id="a544e-117">所有者</span><span class="sxs-lookup"><span data-stu-id="a544e-117">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="a544e-118">设备所有权类型。</span><span class="sxs-lookup"><span data-stu-id="a544e-118">Device ownership type.</span></span> <span data-ttu-id="a544e-119">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="a544e-119">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a544e-120">action</span><span class="sxs-lookup"><span data-stu-id="a544e-120">action</span></span>|[<span data-ttu-id="a544e-121">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="a544e-121">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="a544e-122">设备操作。</span><span class="sxs-lookup"><span data-stu-id="a544e-122">Device Action.</span></span> <span data-ttu-id="a544e-123">可取值为：`unknown`、`remove`、`reset`。</span><span class="sxs-lookup"><span data-stu-id="a544e-123">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a544e-124">关系</span><span class="sxs-lookup"><span data-stu-id="a544e-124">Relationships</span></span>
<span data-ttu-id="a544e-125">无</span><span class="sxs-lookup"><span data-stu-id="a544e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a544e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a544e-126">JSON Representation</span></span>
<span data-ttu-id="a544e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a544e-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```



