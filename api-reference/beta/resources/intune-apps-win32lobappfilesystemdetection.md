---
title: win32LobAppFileSystemDetection 资源类型
description: 包含用于检测 Win32 应用程序的文件或文件夹路径
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e899a9caa5e4f21292ec56c5595bc77d3b68bcc2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803246"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="4a58e-103">win32LobAppFileSystemDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a58e-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="4a58e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a58e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a58e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a58e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a58e-106">包含用于检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="4a58e-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="4a58e-107">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="4a58e-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a58e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a58e-108">Properties</span></span>
|<span data-ttu-id="4a58e-109">属性</span><span class="sxs-lookup"><span data-stu-id="4a58e-109">Property</span></span>|<span data-ttu-id="4a58e-110">类型</span><span class="sxs-lookup"><span data-stu-id="4a58e-110">Type</span></span>|<span data-ttu-id="4a58e-111">说明</span><span class="sxs-lookup"><span data-stu-id="4a58e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a58e-112">路径</span><span class="sxs-lookup"><span data-stu-id="4a58e-112">path</span></span>|<span data-ttu-id="4a58e-113">String</span><span class="sxs-lookup"><span data-stu-id="4a58e-113">String</span></span>|<span data-ttu-id="4a58e-114">用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="4a58e-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="4a58e-115">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="4a58e-115">fileOrFolderName</span></span>|<span data-ttu-id="4a58e-116">String</span><span class="sxs-lookup"><span data-stu-id="4a58e-116">String</span></span>|<span data-ttu-id="4a58e-117">要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="4a58e-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="4a58e-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="4a58e-118">check32BitOn64System</span></span>|<span data-ttu-id="4a58e-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="4a58e-119">Boolean</span></span>|<span data-ttu-id="4a58e-120">一个指示此文件或文件夹是否用于检查64位系统上的32位应用程序的值</span><span class="sxs-lookup"><span data-stu-id="4a58e-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="4a58e-121">detectionType</span><span class="sxs-lookup"><span data-stu-id="4a58e-121">detectionType</span></span>|[<span data-ttu-id="4a58e-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="4a58e-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="4a58e-123">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="4a58e-123">The file system detection type.</span></span> <span data-ttu-id="4a58e-124">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB` 或 `doesNotExist`。</span><span class="sxs-lookup"><span data-stu-id="4a58e-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="4a58e-125">operator</span><span class="sxs-lookup"><span data-stu-id="4a58e-125">operator</span></span>|[<span data-ttu-id="4a58e-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="4a58e-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="4a58e-127">用于文件或文件夹检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="4a58e-127">The operator for file or folder detection.</span></span> <span data-ttu-id="4a58e-128">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="4a58e-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="4a58e-129">detectionValue</span><span class="sxs-lookup"><span data-stu-id="4a58e-129">detectionValue</span></span>|<span data-ttu-id="4a58e-130">String</span><span class="sxs-lookup"><span data-stu-id="4a58e-130">String</span></span>|<span data-ttu-id="4a58e-131">文件或文件夹检测值</span><span class="sxs-lookup"><span data-stu-id="4a58e-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a58e-132">关系</span><span class="sxs-lookup"><span data-stu-id="4a58e-132">Relationships</span></span>
<span data-ttu-id="4a58e-133">无</span><span class="sxs-lookup"><span data-stu-id="4a58e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a58e-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a58e-134">JSON Representation</span></span>
<span data-ttu-id="4a58e-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a58e-135">Here is a JSON representation of the resource.</span></span>
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





