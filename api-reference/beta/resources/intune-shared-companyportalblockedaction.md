---
title: companyPortalBlockedAction 资源类型
description: 按平台和设备所有权类型对公司门户的阻止的操作
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e456ba03de299a04a1434c7a19871aa908274b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723769"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="0e5ed-103">companyPortalBlockedAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e5ed-103">companyPortalBlockedAction resource type</span></span>

<span data-ttu-id="0e5ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e5ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e5ed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e5ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e5ed-107">按平台和设备所有权类型对公司门户的阻止的操作</span><span class="sxs-lookup"><span data-stu-id="0e5ed-107">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="0e5ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e5ed-108">Properties</span></span>
|<span data-ttu-id="0e5ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e5ed-109">Property</span></span>|<span data-ttu-id="0e5ed-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e5ed-110">Type</span></span>|<span data-ttu-id="0e5ed-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e5ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e5ed-112">平台</span><span class="sxs-lookup"><span data-stu-id="0e5ed-112">platform</span></span>|[<span data-ttu-id="0e5ed-113">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="0e5ed-113">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="0e5ed-114">设备 OS/平台。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-114">Device OS/Platform.</span></span> <span data-ttu-id="0e5ed-115">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-115">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="0e5ed-116">所有者</span><span class="sxs-lookup"><span data-stu-id="0e5ed-116">ownerType</span></span>|[<span data-ttu-id="0e5ed-117">所有者</span><span class="sxs-lookup"><span data-stu-id="0e5ed-117">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="0e5ed-118">设备所有权类型。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-118">Device ownership type.</span></span> <span data-ttu-id="0e5ed-119">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-119">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="0e5ed-120">action</span><span class="sxs-lookup"><span data-stu-id="0e5ed-120">action</span></span>|[<span data-ttu-id="0e5ed-121">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="0e5ed-121">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="0e5ed-122">设备操作。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-122">Device Action.</span></span> <span data-ttu-id="0e5ed-123">可取值为：`unknown`、`remove`、`reset`。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-123">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e5ed-124">关系</span><span class="sxs-lookup"><span data-stu-id="0e5ed-124">Relationships</span></span>
<span data-ttu-id="0e5ed-125">无</span><span class="sxs-lookup"><span data-stu-id="0e5ed-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e5ed-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e5ed-126">JSON Representation</span></span>
<span data-ttu-id="0e5ed-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e5ed-127">Here is a JSON representation of the resource.</span></span>
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





