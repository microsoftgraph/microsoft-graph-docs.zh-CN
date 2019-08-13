---
title: win32LobAppRegistryRequirement 资源类型
description: 包含用于检测 Win32 应用程序的注册表属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 21a3befbe695af82688da842793f2f136ae2c79d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335520"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="6ed5d-103">win32LobAppRegistryRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ed5d-103">win32LobAppRegistryRequirement resource type</span></span>

> <span data-ttu-id="6ed5d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ed5d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ed5d-106">包含用于检测 Win32 应用程序的注册表属性</span><span class="sxs-lookup"><span data-stu-id="6ed5d-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="6ed5d-107">继承自[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="6ed5d-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ed5d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ed5d-108">Properties</span></span>
|<span data-ttu-id="6ed5d-109">属性</span><span class="sxs-lookup"><span data-stu-id="6ed5d-109">Property</span></span>|<span data-ttu-id="6ed5d-110">类型</span><span class="sxs-lookup"><span data-stu-id="6ed5d-110">Type</span></span>|<span data-ttu-id="6ed5d-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ed5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ed5d-112">operator</span><span class="sxs-lookup"><span data-stu-id="6ed5d-112">operator</span></span>|[<span data-ttu-id="6ed5d-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="6ed5d-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="6ed5d-114">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="6ed5d-115">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="6ed5d-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="6ed5d-116">detectionValue</span></span>|<span data-ttu-id="6ed5d-117">String</span><span class="sxs-lookup"><span data-stu-id="6ed5d-117">String</span></span>|<span data-ttu-id="6ed5d-118">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="6ed5d-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="6ed5d-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="6ed5d-119">check32BitOn64System</span></span>|<span data-ttu-id="6ed5d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ed5d-120">Boolean</span></span>|<span data-ttu-id="6ed5d-121">一个值, 该值指示此注册表路径是否用于检查64位系统上的32位应用</span><span class="sxs-lookup"><span data-stu-id="6ed5d-121">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="6ed5d-122">keyPath</span><span class="sxs-lookup"><span data-stu-id="6ed5d-122">keyPath</span></span>|<span data-ttu-id="6ed5d-123">String</span><span class="sxs-lookup"><span data-stu-id="6ed5d-123">String</span></span>|<span data-ttu-id="6ed5d-124">用于检测 Win32 业务线 (LoB) 应用程序的注册表项路径</span><span class="sxs-lookup"><span data-stu-id="6ed5d-124">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="6ed5d-125">等值</span><span class="sxs-lookup"><span data-stu-id="6ed5d-125">valueName</span></span>|<span data-ttu-id="6ed5d-126">String</span><span class="sxs-lookup"><span data-stu-id="6ed5d-126">String</span></span>|<span data-ttu-id="6ed5d-127">注册表值名称</span><span class="sxs-lookup"><span data-stu-id="6ed5d-127">The registry value name</span></span>|
|<span data-ttu-id="6ed5d-128">detectionType</span><span class="sxs-lookup"><span data-stu-id="6ed5d-128">detectionType</span></span>|[<span data-ttu-id="6ed5d-129">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="6ed5d-129">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="6ed5d-130">注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-130">The registry data detection type.</span></span> <span data-ttu-id="6ed5d-131">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-131">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ed5d-132">关系</span><span class="sxs-lookup"><span data-stu-id="6ed5d-132">Relationships</span></span>
<span data-ttu-id="6ed5d-133">无</span><span class="sxs-lookup"><span data-stu-id="6ed5d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ed5d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ed5d-134">JSON Representation</span></span>
<span data-ttu-id="6ed5d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ed5d-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRequirement",
  "operator": "String",
  "detectionValue": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```



