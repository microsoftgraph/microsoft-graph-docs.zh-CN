---
title: win32LobAppRequirement 资源类型
description: 用于检测 Win32 应用程序的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76f907b9eefe8d9b62aca05bc27dd92d7c8f61cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280723"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="2b999-103">win32LobAppRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b999-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="2b999-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b999-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b999-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b999-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b999-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b999-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b999-107">用于检测 Win32 应用程序的基类</span><span class="sxs-lookup"><span data-stu-id="2b999-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="2b999-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b999-108">Properties</span></span>
|<span data-ttu-id="2b999-109">属性</span><span class="sxs-lookup"><span data-stu-id="2b999-109">Property</span></span>|<span data-ttu-id="2b999-110">类型</span><span class="sxs-lookup"><span data-stu-id="2b999-110">Type</span></span>|<span data-ttu-id="2b999-111">Description</span><span class="sxs-lookup"><span data-stu-id="2b999-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b999-112">operator</span><span class="sxs-lookup"><span data-stu-id="2b999-112">operator</span></span>|[<span data-ttu-id="2b999-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="2b999-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="2b999-114">用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="2b999-114">The operator for detection.</span></span> <span data-ttu-id="2b999-115">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="2b999-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2b999-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="2b999-116">detectionValue</span></span>|<span data-ttu-id="2b999-117">字符串</span><span class="sxs-lookup"><span data-stu-id="2b999-117">String</span></span>|<span data-ttu-id="2b999-118">检测值</span><span class="sxs-lookup"><span data-stu-id="2b999-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b999-119">关系</span><span class="sxs-lookup"><span data-stu-id="2b999-119">Relationships</span></span>
<span data-ttu-id="2b999-120">无</span><span class="sxs-lookup"><span data-stu-id="2b999-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b999-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b999-121">JSON Representation</span></span>
<span data-ttu-id="2b999-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b999-122">Here is a JSON representation of the resource.</span></span>
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




