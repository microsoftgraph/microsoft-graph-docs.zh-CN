---
title: win32LobAppFileSystemRule 资源类型
description: 用于存储 Win32 LOB 应用程序的文件或文件夹规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e45db436201b339f075f35d3865c8d0c84f1ea6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274031"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="401b4-103">win32LobAppFileSystemRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="401b4-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="401b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="401b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="401b4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="401b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="401b4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="401b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="401b4-107">用于存储 Win32 LOB 应用程序的文件或文件夹规则数据的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="401b4-107">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="401b4-108">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="401b4-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="401b4-109">属性</span><span class="sxs-lookup"><span data-stu-id="401b4-109">Properties</span></span>
|<span data-ttu-id="401b4-110">属性</span><span class="sxs-lookup"><span data-stu-id="401b4-110">Property</span></span>|<span data-ttu-id="401b4-111">类型</span><span class="sxs-lookup"><span data-stu-id="401b4-111">Type</span></span>|<span data-ttu-id="401b4-112">说明</span><span class="sxs-lookup"><span data-stu-id="401b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="401b4-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="401b4-113">ruleType</span></span>|[<span data-ttu-id="401b4-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="401b4-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="401b4-115">指示规则用途的规则类型。</span><span class="sxs-lookup"><span data-stu-id="401b4-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="401b4-116">继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。</span><span class="sxs-lookup"><span data-stu-id="401b4-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="401b4-117">可取值为：`detection`、`requirement`。</span><span class="sxs-lookup"><span data-stu-id="401b4-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="401b4-118">路径</span><span class="sxs-lookup"><span data-stu-id="401b4-118">path</span></span>|<span data-ttu-id="401b4-119">String</span><span class="sxs-lookup"><span data-stu-id="401b4-119">String</span></span>|<span data-ttu-id="401b4-120">要查找的文件或文件夹路径。</span><span class="sxs-lookup"><span data-stu-id="401b4-120">The file or folder path to look up.</span></span>|
|<span data-ttu-id="401b4-121">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="401b4-121">fileOrFolderName</span></span>|<span data-ttu-id="401b4-122">字符串</span><span class="sxs-lookup"><span data-stu-id="401b4-122">String</span></span>|<span data-ttu-id="401b4-123">要查找的文件或文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="401b4-123">The file or folder name to look up.</span></span>|
|<span data-ttu-id="401b4-124">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="401b4-124">check32BitOn64System</span></span>|<span data-ttu-id="401b4-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="401b4-125">Boolean</span></span>|<span data-ttu-id="401b4-126">一个值，指示是否在64位系统上展开32位上下文中的环境变量。</span><span class="sxs-lookup"><span data-stu-id="401b4-126">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="401b4-127">operationType</span><span class="sxs-lookup"><span data-stu-id="401b4-127">operationType</span></span>|[<span data-ttu-id="401b4-128">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="401b4-128">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="401b4-129">文件系统操作类型。</span><span class="sxs-lookup"><span data-stu-id="401b4-129">The file system operation type.</span></span> <span data-ttu-id="401b4-130">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB` 或 `doesNotExist`。</span><span class="sxs-lookup"><span data-stu-id="401b4-130">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="401b4-131">operator</span><span class="sxs-lookup"><span data-stu-id="401b4-131">operator</span></span>|[<span data-ttu-id="401b4-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="401b4-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="401b4-133">用于文件或文件夹检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="401b4-133">The operator for file or folder detection.</span></span> <span data-ttu-id="401b4-134">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="401b4-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="401b4-135">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="401b4-135">comparisonValue</span></span>|<span data-ttu-id="401b4-136">字符串</span><span class="sxs-lookup"><span data-stu-id="401b4-136">String</span></span>|<span data-ttu-id="401b4-137">文件或文件夹的比较值。</span><span class="sxs-lookup"><span data-stu-id="401b4-137">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="401b4-138">关系</span><span class="sxs-lookup"><span data-stu-id="401b4-138">Relationships</span></span>
<span data-ttu-id="401b4-139">无</span><span class="sxs-lookup"><span data-stu-id="401b4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="401b4-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="401b4-140">JSON Representation</span></span>
<span data-ttu-id="401b4-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="401b4-141">Here is a JSON representation of the resource.</span></span>
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




