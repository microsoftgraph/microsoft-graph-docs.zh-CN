---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4fda7cc98c8041aad45a0ef8453affc9af34edc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501225"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="5a875-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="5a875-103">educationPowerSchoolDataProvider resource</span></span>

<span data-ttu-id="5a875-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5a875-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a875-105">用于在将[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="5a875-105">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="5a875-106">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="5a875-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a875-107">属性</span><span class="sxs-lookup"><span data-stu-id="5a875-107">Properties</span></span>

| <span data-ttu-id="5a875-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a875-108">Property</span></span> | <span data-ttu-id="5a875-109">类型</span><span class="sxs-lookup"><span data-stu-id="5a875-109">Type</span></span> | <span data-ttu-id="5a875-110">说明</span><span class="sxs-lookup"><span data-stu-id="5a875-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5a875-111">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="5a875-111">**connectionUrl**</span></span> | <span data-ttu-id="5a875-112">String</span><span class="sxs-lookup"><span data-stu-id="5a875-112">String</span></span> | <span data-ttu-id="5a875-113">指向 PowerSchool 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="5a875-113">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="5a875-114">**clientId**</span><span class="sxs-lookup"><span data-stu-id="5a875-114">**clientId**</span></span> | <span data-ttu-id="5a875-115">String</span><span class="sxs-lookup"><span data-stu-id="5a875-115">String</span></span> |  <span data-ttu-id="5a875-116">用于连接到 PowerSchool 的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="5a875-116">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="5a875-117">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="5a875-117">**clientSecret**</span></span> | <span data-ttu-id="5a875-118">String</span><span class="sxs-lookup"><span data-stu-id="5a875-118">String</span></span> |  <span data-ttu-id="5a875-119">用于对与 PowerSchool 实例的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="5a875-119">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="5a875-120">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="5a875-120">**schoolsIds**</span></span> | <span data-ttu-id="5a875-121">String 集合</span><span class="sxs-lookup"><span data-stu-id="5a875-121">String collection</span></span> |  <span data-ttu-id="5a875-122">要同步的学校列表。</span><span class="sxs-lookup"><span data-stu-id="5a875-122">The list of schools to sync.</span></span> |
| <span data-ttu-id="5a875-123">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="5a875-123">**schoolYear**</span></span> | <span data-ttu-id="5a875-124">String</span><span class="sxs-lookup"><span data-stu-id="5a875-124">String</span></span> |  <span data-ttu-id="5a875-125">要同步的学校年。</span><span class="sxs-lookup"><span data-stu-id="5a875-125">The school year to sync.</span></span> |
| <span data-ttu-id="5a875-126">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="5a875-126">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="5a875-127">布尔</span><span class="sxs-lookup"><span data-stu-id="5a875-127">Boolean</span></span> |  <span data-ttu-id="5a875-128">指示源是否具有单个学生或教师的多个标识符。</span><span class="sxs-lookup"><span data-stu-id="5a875-128">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="5a875-129">**操作**</span><span class="sxs-lookup"><span data-stu-id="5a875-129">**customizations**</span></span> | [<span data-ttu-id="5a875-130">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="5a875-130">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="5a875-131">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="5a875-131">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a875-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a875-132">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
