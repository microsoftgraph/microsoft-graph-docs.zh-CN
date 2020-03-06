---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f49f5651c6e4f7bea1eb4650e9252c397cc2a930
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533325"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8719f-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8719f-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="8719f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8719f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8719f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8719f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8719f-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8719f-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="8719f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8719f-107">Properties</span></span>
|<span data-ttu-id="8719f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8719f-108">Property</span></span>|<span data-ttu-id="8719f-109">类型</span><span class="sxs-lookup"><span data-stu-id="8719f-109">Type</span></span>|<span data-ttu-id="8719f-110">说明</span><span class="sxs-lookup"><span data-stu-id="8719f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8719f-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="8719f-111">subjectName</span></span>|<span data-ttu-id="8719f-112">String</span><span class="sxs-lookup"><span data-stu-id="8719f-112">String</span></span>|<span data-ttu-id="8719f-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="8719f-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8719f-114">说明</span><span class="sxs-lookup"><span data-stu-id="8719f-114">description</span></span>|<span data-ttu-id="8719f-115">字符串</span><span class="sxs-lookup"><span data-stu-id="8719f-115">String</span></span>|<span data-ttu-id="8719f-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="8719f-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8719f-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8719f-117">expirationDateTime</span></span>|<span data-ttu-id="8719f-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8719f-118">DateTimeOffset</span></span>|<span data-ttu-id="8719f-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="8719f-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8719f-120">证书</span><span class="sxs-lookup"><span data-stu-id="8719f-120">certificate</span></span>|<span data-ttu-id="8719f-121">Binary</span><span class="sxs-lookup"><span data-stu-id="8719f-121">Binary</span></span>|<span data-ttu-id="8719f-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="8719f-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8719f-123">关系</span><span class="sxs-lookup"><span data-stu-id="8719f-123">Relationships</span></span>
<span data-ttu-id="8719f-124">无</span><span class="sxs-lookup"><span data-stu-id="8719f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8719f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8719f-125">JSON Representation</span></span>
<span data-ttu-id="8719f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8719f-126">Here is a JSON representation of the resource.</span></span>
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




