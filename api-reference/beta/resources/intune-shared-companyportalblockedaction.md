---
title: companyPortalBlockedAction 资源类型
description: 按平台和设备所有权类型对公司门户的阻止的操作
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ed24dc039742ef7c0412fcd8a67f1a460062c7f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088278"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="1172d-103">companyPortalBlockedAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="1172d-103">companyPortalBlockedAction resource type</span></span>

> <span data-ttu-id="1172d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1172d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1172d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1172d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1172d-106">按平台和设备所有权类型对公司门户的阻止的操作</span><span class="sxs-lookup"><span data-stu-id="1172d-106">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="1172d-107">属性</span><span class="sxs-lookup"><span data-stu-id="1172d-107">Properties</span></span>
|<span data-ttu-id="1172d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1172d-108">Property</span></span>|<span data-ttu-id="1172d-109">类型</span><span class="sxs-lookup"><span data-stu-id="1172d-109">Type</span></span>|<span data-ttu-id="1172d-110">描述</span><span class="sxs-lookup"><span data-stu-id="1172d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1172d-111">platform</span><span class="sxs-lookup"><span data-stu-id="1172d-111">platform</span></span>|[<span data-ttu-id="1172d-112">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="1172d-112">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="1172d-113">设备 OS/平台。</span><span class="sxs-lookup"><span data-stu-id="1172d-113">Device OS/Platform.</span></span> <span data-ttu-id="1172d-114">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="1172d-114">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="1172d-115">所有者</span><span class="sxs-lookup"><span data-stu-id="1172d-115">ownerType</span></span>|[<span data-ttu-id="1172d-116">所有者</span><span class="sxs-lookup"><span data-stu-id="1172d-116">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="1172d-117">设备所有权类型。</span><span class="sxs-lookup"><span data-stu-id="1172d-117">Device ownership type.</span></span> <span data-ttu-id="1172d-118">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="1172d-118">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="1172d-119">action</span><span class="sxs-lookup"><span data-stu-id="1172d-119">action</span></span>|[<span data-ttu-id="1172d-120">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="1172d-120">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="1172d-121">设备操作。</span><span class="sxs-lookup"><span data-stu-id="1172d-121">Device Action.</span></span> <span data-ttu-id="1172d-122">可取值为：`unknown`、`remove`、`reset`。</span><span class="sxs-lookup"><span data-stu-id="1172d-122">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1172d-123">关系</span><span class="sxs-lookup"><span data-stu-id="1172d-123">Relationships</span></span>
<span data-ttu-id="1172d-124">无</span><span class="sxs-lookup"><span data-stu-id="1172d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1172d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1172d-125">JSON Representation</span></span>
<span data-ttu-id="1172d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1172d-126">Here is a JSON representation of the resource.</span></span>
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



