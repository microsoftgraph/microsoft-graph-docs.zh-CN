---
title: win32LobAppRequirement 资源类型
description: 用于检测 Win32 应用程序的基类
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91c8a23170ba18e2c5c8ec3a3890e548a27df9cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797561"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="f371c-103">win32LobAppRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="f371c-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="f371c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f371c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f371c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f371c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f371c-106">用于检测 Win32 应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="f371c-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="f371c-107">属性</span><span class="sxs-lookup"><span data-stu-id="f371c-107">Properties</span></span>
|<span data-ttu-id="f371c-108">属性</span><span class="sxs-lookup"><span data-stu-id="f371c-108">Property</span></span>|<span data-ttu-id="f371c-109">类型</span><span class="sxs-lookup"><span data-stu-id="f371c-109">Type</span></span>|<span data-ttu-id="f371c-110">说明</span><span class="sxs-lookup"><span data-stu-id="f371c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f371c-111">operator</span><span class="sxs-lookup"><span data-stu-id="f371c-111">operator</span></span>|[<span data-ttu-id="f371c-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f371c-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f371c-113">用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="f371c-113">The operator for detection.</span></span> <span data-ttu-id="f371c-114">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="f371c-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f371c-115">detectionValue</span><span class="sxs-lookup"><span data-stu-id="f371c-115">detectionValue</span></span>|<span data-ttu-id="f371c-116">String</span><span class="sxs-lookup"><span data-stu-id="f371c-116">String</span></span>|<span data-ttu-id="f371c-117">检测值</span><span class="sxs-lookup"><span data-stu-id="f371c-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f371c-118">关系</span><span class="sxs-lookup"><span data-stu-id="f371c-118">Relationships</span></span>
<span data-ttu-id="f371c-119">无</span><span class="sxs-lookup"><span data-stu-id="f371c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f371c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f371c-120">JSON Representation</span></span>
<span data-ttu-id="f371c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f371c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRequirement",
  "operator": "String",
  "detectionValue": "String"
}
```



