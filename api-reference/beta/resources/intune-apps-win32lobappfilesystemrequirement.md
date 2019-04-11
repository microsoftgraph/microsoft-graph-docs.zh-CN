---
title: win32LobAppFileSystemRequirement 资源类型
description: 包含用于检测 Win32 应用程序的文件或文件夹路径
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efd0a202d6db1711caa4c7341367d3d1afe85038
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809178"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="ff7fd-103">win32LobAppFileSystemRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff7fd-103">win32LobAppFileSystemRequirement resource type</span></span>

> <span data-ttu-id="ff7fd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff7fd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff7fd-106">包含用于检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="ff7fd-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="ff7fd-107">继承自[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="ff7fd-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff7fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff7fd-108">Properties</span></span>
|<span data-ttu-id="ff7fd-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff7fd-109">Property</span></span>|<span data-ttu-id="ff7fd-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff7fd-110">Type</span></span>|<span data-ttu-id="ff7fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff7fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff7fd-112">operator</span><span class="sxs-lookup"><span data-stu-id="ff7fd-112">operator</span></span>|[<span data-ttu-id="ff7fd-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="ff7fd-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="ff7fd-114">从[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="ff7fd-115">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="ff7fd-116">detectionValue</span><span class="sxs-lookup"><span data-stu-id="ff7fd-116">detectionValue</span></span>|<span data-ttu-id="ff7fd-117">String</span><span class="sxs-lookup"><span data-stu-id="ff7fd-117">String</span></span>|<span data-ttu-id="ff7fd-118">从[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="ff7fd-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="ff7fd-119">路径</span><span class="sxs-lookup"><span data-stu-id="ff7fd-119">path</span></span>|<span data-ttu-id="ff7fd-120">String</span><span class="sxs-lookup"><span data-stu-id="ff7fd-120">String</span></span>|<span data-ttu-id="ff7fd-121">用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="ff7fd-121">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="ff7fd-122">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="ff7fd-122">fileOrFolderName</span></span>|<span data-ttu-id="ff7fd-123">String</span><span class="sxs-lookup"><span data-stu-id="ff7fd-123">String</span></span>|<span data-ttu-id="ff7fd-124">要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="ff7fd-124">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="ff7fd-125">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="ff7fd-125">check32BitOn64System</span></span>|<span data-ttu-id="ff7fd-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="ff7fd-126">Boolean</span></span>|<span data-ttu-id="ff7fd-127">一个指示此文件或文件夹是否用于检查64位系统上的32位应用程序的值</span><span class="sxs-lookup"><span data-stu-id="ff7fd-127">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="ff7fd-128">detectionType</span><span class="sxs-lookup"><span data-stu-id="ff7fd-128">detectionType</span></span>|[<span data-ttu-id="ff7fd-129">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="ff7fd-129">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="ff7fd-130">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-130">The file system detection type.</span></span> <span data-ttu-id="ff7fd-131">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`、`doesNotExist`。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-131">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff7fd-132">关系</span><span class="sxs-lookup"><span data-stu-id="ff7fd-132">Relationships</span></span>
<span data-ttu-id="ff7fd-133">无</span><span class="sxs-lookup"><span data-stu-id="ff7fd-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff7fd-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff7fd-134">JSON Representation</span></span>
<span data-ttu-id="ff7fd-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff7fd-135">Here is a JSON representation of the resource.</span></span>
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





