---
title: win32LobAppRequirement 资源类型
description: 用于检测 Win32 应用程序的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee8593603f00a06fc47540d2829ef851cc99facb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949505"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="72845-103">win32LobAppRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="72845-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="72845-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="72845-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72845-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72845-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72845-106">用于检测 Win32 应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="72845-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="72845-107">属性</span><span class="sxs-lookup"><span data-stu-id="72845-107">Properties</span></span>
|<span data-ttu-id="72845-108">属性</span><span class="sxs-lookup"><span data-stu-id="72845-108">Property</span></span>|<span data-ttu-id="72845-109">类型</span><span class="sxs-lookup"><span data-stu-id="72845-109">Type</span></span>|<span data-ttu-id="72845-110">说明</span><span class="sxs-lookup"><span data-stu-id="72845-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72845-111">operator</span><span class="sxs-lookup"><span data-stu-id="72845-111">operator</span></span>|[<span data-ttu-id="72845-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="72845-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="72845-113">用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="72845-113">The operator for detection.</span></span> <span data-ttu-id="72845-114">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="72845-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="72845-115">detectionValue</span><span class="sxs-lookup"><span data-stu-id="72845-115">detectionValue</span></span>|<span data-ttu-id="72845-116">String</span><span class="sxs-lookup"><span data-stu-id="72845-116">String</span></span>|<span data-ttu-id="72845-117">检测值</span><span class="sxs-lookup"><span data-stu-id="72845-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="72845-118">关系</span><span class="sxs-lookup"><span data-stu-id="72845-118">Relationships</span></span>
<span data-ttu-id="72845-119">无</span><span class="sxs-lookup"><span data-stu-id="72845-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72845-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72845-120">JSON Representation</span></span>
<span data-ttu-id="72845-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72845-121">Here is a JSON representation of the resource.</span></span>
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




