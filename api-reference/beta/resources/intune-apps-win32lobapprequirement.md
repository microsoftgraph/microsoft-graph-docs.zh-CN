---
title: win32LobAppRequirement 资源类型
description: 用于检测 Win32 应用程序的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a4254b405020bb1485b0b19e4521eda2556a680
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706189"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="db215-103">win32LobAppRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="db215-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="db215-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db215-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db215-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db215-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db215-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db215-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db215-107">用于检测 Win32 应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="db215-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="db215-108">属性</span><span class="sxs-lookup"><span data-stu-id="db215-108">Properties</span></span>
|<span data-ttu-id="db215-109">属性</span><span class="sxs-lookup"><span data-stu-id="db215-109">Property</span></span>|<span data-ttu-id="db215-110">类型</span><span class="sxs-lookup"><span data-stu-id="db215-110">Type</span></span>|<span data-ttu-id="db215-111">说明</span><span class="sxs-lookup"><span data-stu-id="db215-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db215-112">operator</span><span class="sxs-lookup"><span data-stu-id="db215-112">operator</span></span>|[<span data-ttu-id="db215-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="db215-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="db215-114">用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="db215-114">The operator for detection.</span></span> <span data-ttu-id="db215-115">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="db215-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="db215-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="db215-116">detectionValue</span></span>|<span data-ttu-id="db215-117">String</span><span class="sxs-lookup"><span data-stu-id="db215-117">String</span></span>|<span data-ttu-id="db215-118">检测值</span><span class="sxs-lookup"><span data-stu-id="db215-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="db215-119">关系</span><span class="sxs-lookup"><span data-stu-id="db215-119">Relationships</span></span>
<span data-ttu-id="db215-120">无</span><span class="sxs-lookup"><span data-stu-id="db215-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db215-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db215-121">JSON Representation</span></span>
<span data-ttu-id="db215-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db215-122">Here is a JSON representation of the resource.</span></span>
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





