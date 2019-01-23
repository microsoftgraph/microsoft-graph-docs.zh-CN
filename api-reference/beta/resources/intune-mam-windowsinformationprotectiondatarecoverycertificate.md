---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5606906cbec0122137faf3cb454edec785c42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405798"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="e06af-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="e06af-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="e06af-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e06af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e06af-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e06af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e06af-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e06af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e06af-107">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="e06af-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="e06af-108">属性</span><span class="sxs-lookup"><span data-stu-id="e06af-108">Properties</span></span>
|<span data-ttu-id="e06af-109">属性</span><span class="sxs-lookup"><span data-stu-id="e06af-109">Property</span></span>|<span data-ttu-id="e06af-110">类型</span><span class="sxs-lookup"><span data-stu-id="e06af-110">Type</span></span>|<span data-ttu-id="e06af-111">说明</span><span class="sxs-lookup"><span data-stu-id="e06af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e06af-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="e06af-112">subjectName</span></span>|<span data-ttu-id="e06af-113">String</span><span class="sxs-lookup"><span data-stu-id="e06af-113">String</span></span>|<span data-ttu-id="e06af-114">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="e06af-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="e06af-115">description</span><span class="sxs-lookup"><span data-stu-id="e06af-115">description</span></span>|<span data-ttu-id="e06af-116">String</span><span class="sxs-lookup"><span data-stu-id="e06af-116">String</span></span>|<span data-ttu-id="e06af-117">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="e06af-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="e06af-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e06af-118">expirationDateTime</span></span>|<span data-ttu-id="e06af-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e06af-119">DateTimeOffset</span></span>|<span data-ttu-id="e06af-120">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="e06af-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="e06af-121">证书</span><span class="sxs-lookup"><span data-stu-id="e06af-121">certificate</span></span>|<span data-ttu-id="e06af-122">Binary</span><span class="sxs-lookup"><span data-stu-id="e06af-122">Binary</span></span>|<span data-ttu-id="e06af-123">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="e06af-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="e06af-124">关系</span><span class="sxs-lookup"><span data-stu-id="e06af-124">Relationships</span></span>
<span data-ttu-id="e06af-125">无</span><span class="sxs-lookup"><span data-stu-id="e06af-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e06af-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e06af-126">JSON Representation</span></span>
<span data-ttu-id="e06af-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e06af-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




