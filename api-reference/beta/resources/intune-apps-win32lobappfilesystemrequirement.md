---
title: win32LobAppFileSystemRequirement 资源类型
description: 包含用于检测 Win32 应用程序的文件或文件夹路径
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19ffbebea879856af5a00a77ad4329320be3f78f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966623"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="163e9-103">win32LobAppFileSystemRequirement 资源类型</span><span class="sxs-lookup"><span data-stu-id="163e9-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="163e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="163e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="163e9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="163e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="163e9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="163e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="163e9-107">包含用于检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="163e9-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="163e9-108">继承自 [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="163e9-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="163e9-109">属性</span><span class="sxs-lookup"><span data-stu-id="163e9-109">Properties</span></span>
|<span data-ttu-id="163e9-110">属性</span><span class="sxs-lookup"><span data-stu-id="163e9-110">Property</span></span>|<span data-ttu-id="163e9-111">类型</span><span class="sxs-lookup"><span data-stu-id="163e9-111">Type</span></span>|<span data-ttu-id="163e9-112">说明</span><span class="sxs-lookup"><span data-stu-id="163e9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163e9-113">operator</span><span class="sxs-lookup"><span data-stu-id="163e9-113">operator</span></span>|[<span data-ttu-id="163e9-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="163e9-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="163e9-115">从 [Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="163e9-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="163e9-116">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="163e9-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="163e9-117">detectionValue</span><span class="sxs-lookup"><span data-stu-id="163e9-117">detectionValue</span></span>|<span data-ttu-id="163e9-118">String</span><span class="sxs-lookup"><span data-stu-id="163e9-118">String</span></span>|<span data-ttu-id="163e9-119">从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值</span><span class="sxs-lookup"><span data-stu-id="163e9-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="163e9-120">路径</span><span class="sxs-lookup"><span data-stu-id="163e9-120">path</span></span>|<span data-ttu-id="163e9-121">String</span><span class="sxs-lookup"><span data-stu-id="163e9-121">String</span></span>|<span data-ttu-id="163e9-122">用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="163e9-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="163e9-123">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="163e9-123">fileOrFolderName</span></span>|<span data-ttu-id="163e9-124">String</span><span class="sxs-lookup"><span data-stu-id="163e9-124">String</span></span>|<span data-ttu-id="163e9-125">用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="163e9-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="163e9-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="163e9-126">check32BitOn64System</span></span>|<span data-ttu-id="163e9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="163e9-127">Boolean</span></span>|<span data-ttu-id="163e9-128">一个指示此文件或文件夹是否用于检查64位系统上的32位应用程序的值</span><span class="sxs-lookup"><span data-stu-id="163e9-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="163e9-129">detectionType</span><span class="sxs-lookup"><span data-stu-id="163e9-129">detectionType</span></span>|[<span data-ttu-id="163e9-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="163e9-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="163e9-131">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="163e9-131">The file system detection type.</span></span> <span data-ttu-id="163e9-132">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`、`doesNotExist`。</span><span class="sxs-lookup"><span data-stu-id="163e9-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="163e9-133">关系</span><span class="sxs-lookup"><span data-stu-id="163e9-133">Relationships</span></span>
<span data-ttu-id="163e9-134">无</span><span class="sxs-lookup"><span data-stu-id="163e9-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="163e9-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="163e9-135">JSON Representation</span></span>
<span data-ttu-id="163e9-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="163e9-136">Here is a JSON representation of the resource.</span></span>
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






