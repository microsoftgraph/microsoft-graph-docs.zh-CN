---
title: win32LobAppFileSystemDetection 资源类型
description: 包含要检测 Win32 应用程序的文件或文件夹路径
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5fb4e66ce17fb7a964f3210244e2f3a7027c578
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415227"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="89f2c-103">win32LobAppFileSystemDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="89f2c-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="89f2c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="89f2c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="89f2c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89f2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89f2c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89f2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f2c-107">包含要检测 Win32 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="89f2c-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="89f2c-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="89f2c-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89f2c-109">属性</span><span class="sxs-lookup"><span data-stu-id="89f2c-109">Properties</span></span>
|<span data-ttu-id="89f2c-110">属性</span><span class="sxs-lookup"><span data-stu-id="89f2c-110">Property</span></span>|<span data-ttu-id="89f2c-111">类型</span><span class="sxs-lookup"><span data-stu-id="89f2c-111">Type</span></span>|<span data-ttu-id="89f2c-112">说明</span><span class="sxs-lookup"><span data-stu-id="89f2c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f2c-113">路径</span><span class="sxs-lookup"><span data-stu-id="89f2c-113">path</span></span>|<span data-ttu-id="89f2c-114">String</span><span class="sxs-lookup"><span data-stu-id="89f2c-114">String</span></span>|<span data-ttu-id="89f2c-115">要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径</span><span class="sxs-lookup"><span data-stu-id="89f2c-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="89f2c-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="89f2c-116">fileOrFolderName</span></span>|<span data-ttu-id="89f2c-117">String</span><span class="sxs-lookup"><span data-stu-id="89f2c-117">String</span></span>|<span data-ttu-id="89f2c-118">要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称</span><span class="sxs-lookup"><span data-stu-id="89f2c-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="89f2c-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="89f2c-119">check32BitOn64System</span></span>|<span data-ttu-id="89f2c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="89f2c-120">Boolean</span></span>|<span data-ttu-id="89f2c-121">一个值，该值此文件或文件夹是否检查 64 位系统上的 32 位应用程序</span><span class="sxs-lookup"><span data-stu-id="89f2c-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="89f2c-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="89f2c-122">detectionType</span></span>|[<span data-ttu-id="89f2c-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="89f2c-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="89f2c-124">文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="89f2c-124">The file system detection type.</span></span> <span data-ttu-id="89f2c-125">可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。</span><span class="sxs-lookup"><span data-stu-id="89f2c-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="89f2c-126">operator</span><span class="sxs-lookup"><span data-stu-id="89f2c-126">operator</span></span>|[<span data-ttu-id="89f2c-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="89f2c-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="89f2c-128">文件或文件夹移检测运算符。</span><span class="sxs-lookup"><span data-stu-id="89f2c-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="89f2c-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="89f2c-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="89f2c-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="89f2c-130">detectionValue</span></span>|<span data-ttu-id="89f2c-131">String</span><span class="sxs-lookup"><span data-stu-id="89f2c-131">String</span></span>|<span data-ttu-id="89f2c-132">文件或文件夹检测值</span><span class="sxs-lookup"><span data-stu-id="89f2c-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f2c-133">关系</span><span class="sxs-lookup"><span data-stu-id="89f2c-133">Relationships</span></span>
<span data-ttu-id="89f2c-134">无</span><span class="sxs-lookup"><span data-stu-id="89f2c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f2c-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89f2c-135">JSON Representation</span></span>
<span data-ttu-id="89f2c-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89f2c-136">Here is a JSON representation of the resource.</span></span>
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




