---
title: win32LobAppFileSystemRule 资源类型
description: 用于存储 Win32 LOB 应用的文件或文件夹规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0c8a45a9f3d49c671949a2b5ad3b9bd549ee8d7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752397"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="36cf0-103">win32LobAppFileSystemRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="36cf0-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="36cf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36cf0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36cf0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36cf0-106">用于存储 Win32 LOB 应用的文件或文件夹规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="36cf0-106">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="36cf0-107">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="36cf0-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36cf0-108">属性</span><span class="sxs-lookup"><span data-stu-id="36cf0-108">Properties</span></span>
|<span data-ttu-id="36cf0-109">属性</span><span class="sxs-lookup"><span data-stu-id="36cf0-109">Property</span></span>|<span data-ttu-id="36cf0-110">类型</span><span class="sxs-lookup"><span data-stu-id="36cf0-110">Type</span></span>|<span data-ttu-id="36cf0-111">Description</span><span class="sxs-lookup"><span data-stu-id="36cf0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36cf0-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="36cf0-112">ruleType</span></span>|[<span data-ttu-id="36cf0-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="36cf0-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="36cf0-114">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="36cf0-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="36cf0-115">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="36cf0-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="36cf0-116">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="36cf0-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="36cf0-117">路径</span><span class="sxs-lookup"><span data-stu-id="36cf0-117">path</span></span>|<span data-ttu-id="36cf0-118">String</span><span class="sxs-lookup"><span data-stu-id="36cf0-118">String</span></span>|<span data-ttu-id="36cf0-119">要查找的文件或文件夹路径。</span><span class="sxs-lookup"><span data-stu-id="36cf0-119">The file or folder path to look up.</span></span>|
|<span data-ttu-id="36cf0-120">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="36cf0-120">fileOrFolderName</span></span>|<span data-ttu-id="36cf0-121">String</span><span class="sxs-lookup"><span data-stu-id="36cf0-121">String</span></span>|<span data-ttu-id="36cf0-122">要查找的文件或文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="36cf0-122">The file or folder name to look up.</span></span>|
|<span data-ttu-id="36cf0-123">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="36cf0-123">check32BitOn64System</span></span>|<span data-ttu-id="36cf0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="36cf0-124">Boolean</span></span>|<span data-ttu-id="36cf0-125">一个值，指示是否在 64 位系统上展开 32 位上下文中的环境变量。</span><span class="sxs-lookup"><span data-stu-id="36cf0-125">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="36cf0-126">operationType</span><span class="sxs-lookup"><span data-stu-id="36cf0-126">operationType</span></span>|[<span data-ttu-id="36cf0-127">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="36cf0-127">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="36cf0-128">文件系统操作类型。</span><span class="sxs-lookup"><span data-stu-id="36cf0-128">The file system operation type.</span></span> <span data-ttu-id="36cf0-129">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。</span><span class="sxs-lookup"><span data-stu-id="36cf0-129">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="36cf0-130">operator</span><span class="sxs-lookup"><span data-stu-id="36cf0-130">operator</span></span>|[<span data-ttu-id="36cf0-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="36cf0-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="36cf0-132">文件或文件夹检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="36cf0-132">The operator for file or folder detection.</span></span> <span data-ttu-id="36cf0-133">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="36cf0-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="36cf0-134">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="36cf0-134">comparisonValue</span></span>|<span data-ttu-id="36cf0-135">String</span><span class="sxs-lookup"><span data-stu-id="36cf0-135">String</span></span>|<span data-ttu-id="36cf0-136">文件或文件夹比较值。</span><span class="sxs-lookup"><span data-stu-id="36cf0-136">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36cf0-137">关系</span><span class="sxs-lookup"><span data-stu-id="36cf0-137">Relationships</span></span>
<span data-ttu-id="36cf0-138">无</span><span class="sxs-lookup"><span data-stu-id="36cf0-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36cf0-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36cf0-139">JSON Representation</span></span>
<span data-ttu-id="36cf0-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36cf0-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRule",
  "ruleType": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




