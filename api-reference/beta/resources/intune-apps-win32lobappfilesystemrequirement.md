---
title: win32LobAppFileSystemRequirement 资源类型
description: 包含用于检测 Win32 应用程序的文件或文件夹路径
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f32327461274585941779c45aa7dc2b485acf12f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422986"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="e52bd-103">win32LobAppFileSystemRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="e52bd-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="e52bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e52bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e52bd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e52bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e52bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e52bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e52bd-107">包含用于检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="e52bd-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="e52bd-108">继承自[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="e52bd-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e52bd-109">属性</span><span class="sxs-lookup"><span data-stu-id="e52bd-109">Properties</span></span>
|<span data-ttu-id="e52bd-110">属性</span><span class="sxs-lookup"><span data-stu-id="e52bd-110">Property</span></span>|<span data-ttu-id="e52bd-111">类型</span><span class="sxs-lookup"><span data-stu-id="e52bd-111">Type</span></span>|<span data-ttu-id="e52bd-112">说明</span><span class="sxs-lookup"><span data-stu-id="e52bd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e52bd-113">operator</span><span class="sxs-lookup"><span data-stu-id="e52bd-113">operator</span></span>|[<span data-ttu-id="e52bd-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="e52bd-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="e52bd-115">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="e52bd-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="e52bd-116">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="e52bd-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e52bd-117">detectionValue</span><span class="sxs-lookup"><span data-stu-id="e52bd-117">detectionValue</span></span>|<span data-ttu-id="e52bd-118">String</span><span class="sxs-lookup"><span data-stu-id="e52bd-118">String</span></span>|<span data-ttu-id="e52bd-119">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="e52bd-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="e52bd-120">路径</span><span class="sxs-lookup"><span data-stu-id="e52bd-120">path</span></span>|<span data-ttu-id="e52bd-121">String</span><span class="sxs-lookup"><span data-stu-id="e52bd-121">String</span></span>|<span data-ttu-id="e52bd-122">用于检测 Win32 业务线（LoB）应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="e52bd-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e52bd-123">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="e52bd-123">fileOrFolderName</span></span>|<span data-ttu-id="e52bd-124">String</span><span class="sxs-lookup"><span data-stu-id="e52bd-124">String</span></span>|<span data-ttu-id="e52bd-125">要检测 Win32 业务线（LoB）应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="e52bd-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e52bd-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="e52bd-126">check32BitOn64System</span></span>|<span data-ttu-id="e52bd-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e52bd-127">Boolean</span></span>|<span data-ttu-id="e52bd-128">一个指示此文件或文件夹是否用于检查64位系统上的32位应用程序的值</span><span class="sxs-lookup"><span data-stu-id="e52bd-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="e52bd-129">detectionType</span><span class="sxs-lookup"><span data-stu-id="e52bd-129">detectionType</span></span>|[<span data-ttu-id="e52bd-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="e52bd-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="e52bd-131">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="e52bd-131">The file system detection type.</span></span> <span data-ttu-id="e52bd-132">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`、`doesNotExist`。</span><span class="sxs-lookup"><span data-stu-id="e52bd-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e52bd-133">关系</span><span class="sxs-lookup"><span data-stu-id="e52bd-133">Relationships</span></span>
<span data-ttu-id="e52bd-134">无</span><span class="sxs-lookup"><span data-stu-id="e52bd-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e52bd-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e52bd-135">JSON Representation</span></span>
<span data-ttu-id="e52bd-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e52bd-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```



