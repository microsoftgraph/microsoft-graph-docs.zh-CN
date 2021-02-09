---
title: 配置文件资源类型
description: 表示描述性用户的属性，以及通过 Microsoft Graph 在 Microsoft 365 和第三方服务和体验中显示共享、人员体验的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 542d5907bd1bc467c32ae58836df04a2c62df36f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153513"
---
# <a name="profile-resource-type"></a>配置文件资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中用户的描述属性，例如周年纪念日和教育活动。 这些属性以共享、跨 Microsoft 365 的用户体验以及通过 Microsoft Graph 的第三方服务和体验显示。 

这些属性以编程方式表示为 [配置文件](#relationships)**资源** 的关系。 若要获取其中一个导航属性或为用户创建这些属性的实例，请对该属性使用相应的 GET 或 POST 方法（如果适用）。 请参阅 [下面列出的](#methods) 方法。

## <a name="methods"></a>方法

| 方法                                                                     | 返回类型                                                    | 说明                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [获取个人资料](../api/profile-get.md)                                       | [profile](profile.md)                                          | 读取 profile 对象的属性和关系。                                     |
| [删除个人资料](../api/profile-delete.md)                                 | 无                                                           | 删除 **配置文件** 对象。                                                                 |
| [创建 userAccountInformation](../api/profile-post-accounts.md)           | [userAccountInformation](useraccountinformation.md)            | 通过发布到 **帐户集合创建新的 userAccountInformation** 对象。        |
| [列出帐户](../api/profile-list-accounts.md)                           | [userAccountInformation](useraccountinformation.md) 集合 | 获取 **userAccountInformation** 对象集合。                                          |
| [创建 itemAddress](../api/profile-post-addresses.md)                     | [itemAddress](itemaddress.md)                                  | 通过发布到 **地址集合创建新的 itemAddress。**                         |
| [列出地址](../api/profile-list-addresses.md)                         | [itemAddress](itemaddress.md) 集合                       | 获取 **itemAddress** 对象集合。                                                    |
| [创建 personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | 通过发布到周年日集合创建新的 **personAnniversary。**               |
| [列出周年日](../api/profile-list-anniversaries.md)                 | [personAnniversary](personanniversary.md) 集合           | 获取 **personAnniversary** 对象集合。                                               |
| [创建 personAward](../api/profile-post-awards.md)                        | [personAward](personaward.md)                                  | 通过发布到 **奖励集合创建新的 personAward** 对象。                     |
| [列出奖励](../api/profile-list-awards.md)                               | [personAward](personaward.md) 集合                       | 获取 **personAward** 对象集合。                                                     |
| [创建 personCertification](../api/profile-post-certifications.md)        | [personCertification](personcertification.md)                  | 通过发布到 **认证集合创建新的 personCertification** 对象。     |
| [列出认证](../api/profile-list-certifications.md)               | [personCertification](personcertification.md) 集合       | 获取 **personCertification** 对象集合。                                             |
| [创建 educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | 通过发布到 **educationalActivities** 集合创建新的 **educationalActivity。** |
| [列出 educationalActivities](../api/profile-list-educationalactivities.md) | [educationalActivity](educationalactivity.md) 集合       | 获取 **一个 educationalActivity** 对象集合。                                            |
| [创建 itemEmail](../api/profile-post-emails.md)                          | [itemEmail](itememail.md)                                      | 通过发布到 **电子邮件集合创建新 itemEmail。**                              |
| [列出电子邮件](../api/profile-list-emails.md)                               | [itemEmail](itememail.md) 集合                           | 获取 **itemEmail** 对象集合。                                                      |
| [创建 personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | 通过发布到 **兴趣集合创建新 personInterest。**                      |
| [列出兴趣](../api/profile-list-interests.md)                         | [personInterest](personinterest.md) 集合                 | 获取 **personInterest** 对象集合。                                                  |
| [创建 languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | 通过发布到 **语言集合创建新的 languageProficiency。**                 |
| [列表语言](../api/profile-list-languages.md)                         | [languageProficiency](languageproficiency.md) 集合       | 获取 **languageProficiency** 对象集合。                                             |
| [创建 personName](../api/profile-post-names.md)                          | [personName](personname.md)                                    | 通过发布到 names 集合创建新的 **personName** 对象。                       |
| [列出名称](../api/profile-list-names.md)                                 | [personName](personname.md) 集合                         | 获取 **personName** 对象集合。                                                      |
| [创建 personAnnotation](../api/profile-post-notes.md)                    | [personAnnotation](personannotation.md)                        | 通过发布到 **notes 集合创建新的 personAnnotation** 对象。                 |
| [列出注释](../api/profile-list-notes.md)                                 | [personAnnotation](personannotation.md) 集合             | 获取 **personAnnotation** 对象集合。                                                |
| [创建 itemPatent](../api/profile-post-patents.md)                        | [itemPatent](itempatent.md)                                    | 通过发布到 **专利集合创建新的 itemPatent** 对象。                     |
| [列出专利](../api/profile-list-patents.md)                             | [itemPatent](itempatent.md) 集合                         | 获取 **itemPatent** 对象集合。                                                      |
| [创建 itemPhone](../api/profile-post-phones.md)                          | [itemPhone](itemphone.md)                                      | 通过发布到 phones 集合创建新 itemPhone。                                  |
| [列出电话](../api/profile-list-phones.md)                               | [itemPhone](itemphone.md) 集合                           | 获取 **itemPhone** 对象集合。                                                       |
| [创建 workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | 通过发布到 positions 集合创建新的 workPosition。                            |
| [列出位置](../api/profile-list-positions.md)                         | [workPosition](workposition.md) 集合                     | 获取 **workPosition** 对象集合。                                                    |
| [创建 projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | 通过发布到 **项目集合创建新的 projectParticipation。**                 |
| [列出项目](../api/profile-list-projects.md)                           | [projectParticipation](projectparticipation.md) 集合     | 获取 **projectParticipation** 对象集合。                                            |
| [创建 itemPublication](../api/profile-post-publications.md)              | [itemPublication](itempublication.md)                          | 通过发布到 **出版物集合创建新的 itemPublication** 对象。           |
| [列出出版物](../api/profile-list-publications.md)                   | [itemPublication](itempublication.md) 集合               | 获取 **itemPublication** 对象集合。                                                 |
| [创建 personResponsibility](../api/profile-post-responsibilities.md)     | [personResponsibility](personresponsibility.md)                | 通过发布到 **责任集合创建新的 personResponsibility** 对象。  |
| [列出责任](../api/profile-list-responsibilities.md)           | [personResponsibility](personresponsibility.md) 集合     | 获取 **personResponsibility** 对象集合。                                            |
| [创建 skillProficiency](../api/profile-post-skills.md)                   | [skillProficiency](skillproficiency.md)                        | 通过发布到技能集合创建新的 **skillsProficiency。**                       |
| [列表技能](../api/profile-list-skills.md)                               | [skillProficiency](skillproficiency.md) 集合             | 获取 **一个 skillProficiency** 对象集合。                                                |
| [创建 webAccount](../api/profile-post-webaccounts.md)                    | [webAccount](webaccount.md)                                    | 通过发布到 **webAccounts** 集合创建新的 webAccount。                        |
| [列出 webAccounts](../api/profile-list-webaccounts.md)                     | [webAccount](webaccount.md) 集合                         | 获取 **webAccount** 对象集合。                                                      |
| [创建 personWebsite](../api/profile-post-websites.md)                    | [personWebsite](personwebsite.md)                              | 通过发布到 **网站集合创建新的 personWebsite。**                        |
| [列出网站](../api/profile-list-websites.md)                           | [personWebsite](personwebsite.md) 集合                   | 获取 **personWebsite** 对象集合。                                                   |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id            |String       | 只读。  |

## <a name="relationships"></a>关系

| 关系          | 类型                                                         | 说明                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|账户               |[userAccountInformation](useraccountinformation.md) 集合| 表示专门绑定到用户帐户的信息。                                                             |
|地址              |[itemAddress](itemaddress.md) 集合                      | 表示与用户关联的地址的详细信息。                                                             |
|纪念日          |[personAnniversary](personanniversary.md) 集合          | 表示与某人关联的有意义日期的详细信息。                                                                  |
|奖项                 |[personAward](personaward.md) 集合                      | 表示与某人相关的奖励或奖励的详细信息。                                                                  |
|证书         |[personCertification](personcertification.md) 集合      | 表示与人员关联的认证的详细信息。                                                                  |
|educationalActivities  |[educationalActivity](educationalactivity.md) 集合      | 表示用户提供的与学校、学生、学生或其他教育活动相关的数据。 |
|emails                 |[itemEmail](itememail.md) 集合                          | 表示与用户关联的电子邮件地址的详细信息。                       |
|interests              |[personInterest](personinterest.md) 集合                | 提供有关用户在各种服务中与自己相关联的兴趣的详细信息。             |
|语言              |[languageProficiency](languageproficiency.md) 集合      | 表示有关用户已添加到其配置文件的语言的详细信息。                                    |
|names                  |[personName](personname.md) 集合                        | 表示用户已添加到其配置文件中的名称。                                    |
|注释                  |[personAnnotation](personannotation.md) 集合            | 表示用户已添加到其配置文件的注释。                                    |
|专利                |[itemPatent](itempatent.md) 集合                        | 表示用户已添加到其配置文件中的专利。                                    |
|phones                 |[itemPhone](itemphone.md) 集合                          | 表示与各种服务中的用户关联的电话号码的详细信息。                            |
|positions              |[workPosition](workposition.md) 集合                    | 表示有关与用户配置文件关联的工作职位的详细信息。                                    |
|projects               |[projectParticipation](projectparticipation.md) 集合    | 表示有关与用户关联的项目的详细信息。                                                     |
|出版物           |[itemPublication](itempublication.md) 集合              | 表示用户已添加到其配置文件的任何出版物的详细信息。                                                     |
|responsibilities       |[personResponsibility](personResponsibility.md) 集合    | 表示用户已添加到其配置文件中的责任的详细信息。                                                     |
|skills                 |[skillProficiency](skillproficiency.md) 集合            | 表示有关在各种服务中与用户关联的技能的详细信息。                                   |
|webAccounts            |[webAccount](webaccount.md) 集合                        | 表示用户已指示他们使用或已添加到其用户配置文件的 Web 帐户。                               |
|websites               |[personWebsite](personwebsite.md) 集合                  | 表示与各种服务中的用户关联的网站的详细信息。                                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```


