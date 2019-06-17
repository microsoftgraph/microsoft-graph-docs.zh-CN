---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32a18b25209301e3aeb62aaeaf63f080955cf669
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994529"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="baf44-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="baf44-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="baf44-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="baf44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baf44-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="baf44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baf44-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="baf44-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="baf44-107">属性</span><span class="sxs-lookup"><span data-stu-id="baf44-107">Properties</span></span>
|<span data-ttu-id="baf44-108">属性</span><span class="sxs-lookup"><span data-stu-id="baf44-108">Property</span></span>|<span data-ttu-id="baf44-109">类型</span><span class="sxs-lookup"><span data-stu-id="baf44-109">Type</span></span>|<span data-ttu-id="baf44-110">说明</span><span class="sxs-lookup"><span data-stu-id="baf44-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baf44-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="baf44-111">subjectName</span></span>|<span data-ttu-id="baf44-112">String</span><span class="sxs-lookup"><span data-stu-id="baf44-112">String</span></span>|<span data-ttu-id="baf44-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="baf44-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="baf44-114">说明</span><span class="sxs-lookup"><span data-stu-id="baf44-114">description</span></span>|<span data-ttu-id="baf44-115">String</span><span class="sxs-lookup"><span data-stu-id="baf44-115">String</span></span>|<span data-ttu-id="baf44-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="baf44-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="baf44-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="baf44-117">expirationDateTime</span></span>|<span data-ttu-id="baf44-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baf44-118">DateTimeOffset</span></span>|<span data-ttu-id="baf44-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="baf44-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="baf44-120">证书</span><span class="sxs-lookup"><span data-stu-id="baf44-120">certificate</span></span>|<span data-ttu-id="baf44-121">Binary</span><span class="sxs-lookup"><span data-stu-id="baf44-121">Binary</span></span>|<span data-ttu-id="baf44-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="baf44-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="baf44-123">关系</span><span class="sxs-lookup"><span data-stu-id="baf44-123">Relationships</span></span>
<span data-ttu-id="baf44-124">无</span><span class="sxs-lookup"><span data-stu-id="baf44-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="baf44-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baf44-125">JSON Representation</span></span>
<span data-ttu-id="baf44-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baf44-126">Here is a JSON representation of the resource.</span></span>
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





