---
title: win32LobAppFileSystemDetection 资源类型
description: 包含用于检测 Win32 应用程序的文件或文件夹路径
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d70d24440931c2c5f5ff624856cbdadd0ff097c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033788"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="bc223-103">win32LobAppFileSystemDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc223-103">win32LobAppFileSystemDetection resource type</span></span>

<span data-ttu-id="bc223-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc223-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc223-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc223-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc223-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc223-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc223-107">包含用于检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="bc223-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="bc223-108">继承自 [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="bc223-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc223-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc223-109">Properties</span></span>
|<span data-ttu-id="bc223-110">属性</span><span class="sxs-lookup"><span data-stu-id="bc223-110">Property</span></span>|<span data-ttu-id="bc223-111">类型</span><span class="sxs-lookup"><span data-stu-id="bc223-111">Type</span></span>|<span data-ttu-id="bc223-112">说明</span><span class="sxs-lookup"><span data-stu-id="bc223-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc223-113">路径</span><span class="sxs-lookup"><span data-stu-id="bc223-113">path</span></span>|<span data-ttu-id="bc223-114">String</span><span class="sxs-lookup"><span data-stu-id="bc223-114">String</span></span>|<span data-ttu-id="bc223-115">用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="bc223-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="bc223-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="bc223-116">fileOrFolderName</span></span>|<span data-ttu-id="bc223-117">String</span><span class="sxs-lookup"><span data-stu-id="bc223-117">String</span></span>|<span data-ttu-id="bc223-118">用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="bc223-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="bc223-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="bc223-119">check32BitOn64System</span></span>|<span data-ttu-id="bc223-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="bc223-120">Boolean</span></span>|<span data-ttu-id="bc223-121">一个指示此文件或文件夹是否用于检查64位系统上的32位应用程序的值</span><span class="sxs-lookup"><span data-stu-id="bc223-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="bc223-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="bc223-122">detectionType</span></span>|[<span data-ttu-id="bc223-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="bc223-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="bc223-124">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="bc223-124">The file system detection type.</span></span> <span data-ttu-id="bc223-125">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB` 或 `doesNotExist`。</span><span class="sxs-lookup"><span data-stu-id="bc223-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="bc223-126">operator</span><span class="sxs-lookup"><span data-stu-id="bc223-126">operator</span></span>|[<span data-ttu-id="bc223-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="bc223-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="bc223-128">用于文件或文件夹检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="bc223-128">The operator for file or folder detection.</span></span> <span data-ttu-id="bc223-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="bc223-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="bc223-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="bc223-130">detectionValue</span></span>|<span data-ttu-id="bc223-131">String</span><span class="sxs-lookup"><span data-stu-id="bc223-131">String</span></span>|<span data-ttu-id="bc223-132">文件或文件夹检测值</span><span class="sxs-lookup"><span data-stu-id="bc223-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc223-133">关系</span><span class="sxs-lookup"><span data-stu-id="bc223-133">Relationships</span></span>
<span data-ttu-id="bc223-134">无</span><span class="sxs-lookup"><span data-stu-id="bc223-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc223-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc223-135">JSON Representation</span></span>
<span data-ttu-id="bc223-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc223-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```






