---
title: 使用扩展向资源添加自定义数据
description: Microsoft Graph 提供单一 API 终结点，以便用户能够通过大量资源（如 user 和 message）访问以人为中心的丰富数据和见解。 你还可以使用自己的应用程序数据扩展 Microsoft Graph。 无需使用外部数据存储，即可向 Microsoft Graph 资源添加自定义属性。
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 1433de1b011f76bac8c1f0b0bda2dbbbdeebf288
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821083"
---
# <a name="add-custom-data-to-resources-using-extensions"></a>使用扩展向资源添加自定义数据

Microsoft Graph 提供单一 API 终结点，以便用户能够通过大量资源（如 [user](/graph/api/resources/user) 和 [message](/graph/api/resources/message)）访问以人为中心的丰富数据和见解。 你还可以使用自己的应用程序数据扩展 Microsoft Graph。 无需使用外部数据存储，即可向 Microsoft Graph 资源添加自定义属性。

例如，可能会决定扩展 **user** 资源，让应用处于轻量级水平，并将应用专属的用户配置文件数据存储在 Microsoft Graph 中。 或者，不妨保留应用的现有用户配置文件存储，并仅将应用专属的存储标识符添加到 **user** 资源。

Microsoft Graph 提供两种类型的扩展。选择最适合应用程序需求的扩展类型：

- **开放扩展**：开发人员入门的良好方法。
- **架构扩展**：对于那些关心存储类型化数据，使其架构可发现和可共享，能够进行筛选以及将来能够执行输入数据验证和授权的开发人员而言，这是一种更通用的机制。

> **重要说明：** 不能使用扩展存储敏感的个人身份信息，例如帐户凭据、政府标识号、持卡人数据、财务帐户数据、医疗保健信息或敏感的背景信息。

## <a name="supported-resources"></a>支持的资源

下表列出了支持开放扩展和架构扩展的资源，并指明是处于正式版（GA - 在 v1.0 和 beta 终结点中均可用）阶段，还是处于预览版（仅在 beta 终结点中可用）阶段。

|资源 |开放扩展 |架构扩展 |
|:------- |:------ |:------ |
| [管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true) | 仅供预览 | 仅供预览 |
| [日历事件](/graph/api/resources/event) | GA | GA |
| [设备](/graph/api/resources/device) | GA | GA |
| [组](/graph/api/resources/group) | GA | GA |
| [组日历事件](/graph/api/resources/event) | GA | GA |
| [组对话帖子](/graph/api/resources/post) | GA | GA |
| [邮件](/graph/api/resources/message) | GA | GA |
| [组织](/graph/api/resources/organization) | GA | GA |
| [个人联系人](/graph/api/resources/contact)| GA | GA |
| [用户](/graph/api/resources/user) | GA | GA |
| [待办事项任务](/graph/api/resources/todotask) | GA | GA |
| [待办事项任务列表](/graph/api/resources/todotasklist) | GA | GA |

使用工作或学校帐户登录时，可以对所有这些资源使用扩展。 此外，使用个人帐户登录时，可以对“**事件**”、“**帖子**”、“**组**”、“**邮件**”、“**联系人**”和“**用户**”资源使用扩展。

## <a name="open-extensions"></a>开放扩展

[开放扩展](/graph/api/resources/opentypeextension)（以前称为 Office 365 数据扩展）是提供灵活方法将非类型化应用数据直接添加到资源实例的[开放类型](https://www.odata.org/getting-started/advanced-tutorial/#openType)。

> [!VIDEO https://www.youtube-nocookie.com/embed/ibdlADb8IZc]

开放扩展及其自定义数据可通过资源实例的 **extensions** 导航属性进行访问。
**extensionName** 属性是开放扩展中的 _预定义_ 唯一可写属性。 创建开放扩展时，必须为 **extensionName** 属性分配在租户内唯一的名称。

为此，一种方法是使用反向域名系统 (DNS) 格式，此格式依赖 _用户自己的域_。例如，`Com.Contoso.ContactInfo`。

请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。

可以在资源实例中[创建开放扩展](/graph/api/opentypeextension-post-opentypeextension)，并将自定义数据存储到其中，全都通过同一操作完成（请注意受支持的部分资源的[已知限制](known-issues.md#extensions)）。

随后可以[读取]（/graph/api/opentypeextension-get， [更新](/graph/api/opentypeextension-update)，或 [删除](/graph/api/opentypeextension-delete) 扩展及其数据。

开放扩展示例：[使用开放扩展向用户添加自定义数据](extensibility-open-users.md)

## <a name="schema-extensions"></a>架构扩展


通过[架构扩展](/graph/api/resources/schemaextension)，可以定义一个架构，用来扩展资源类型。 首先，创建架构扩展定义。 然后，利用它通过强类型自定义数据扩展资源实例。 此外，还可以控制架构扩展的[状态](#schema-extensions-lifecycle)，让它可被其他应用发现。 相应地，这些应用可以对自己的数据使用此扩展，并在它的基础之上生成进一步的体验。


> [!VIDEO https://www.youtube-nocookie.com/embed/3MOAlUFNus0]

在创建架构扩展定义时，你必须提供其 **id** 的唯一名称。提供两个命名选项：

- 如果已有通过租户验证的 `.com`、`.net`、`.gov`、`.edu` 或 `.org` 域，可以使用域名和架构名称定义唯一名称，格式如下：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。 例如，如果虚域是 contoso.com，可以定义 `contoso_mySchema` 的 **id**。 此为首选项。
- 如果没有验证的虚域，则可以只设置架构名称的 **id**（不带域名称前缀），例如，`mySchema`。根据所提供的名称，Microsoft Graph 将为你分配一个字符串 ID，采用以下格式：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如，`extkvbmkofy_mySchema`。

可以看到，在 **id** 中此唯一名称用作复杂类型名称，复杂类型将在扩展的资源实例上存储自定义数据。

与开放类型不同，管理架构扩展定义（[列出](/graph/api/schemaextension-list)、[创建](/graph/api/schemaextension-post-schemaextensions)、[获取](/graph/api/schemaextension-get)、[更新](/graph/api/schemaextension-update)及[删除](/graph/api/schemaextension-delete)）和管理其数据（添加、获取、更新及删除数据）是独立的 API 操作集。

由于架构扩展可以在目标资源实例中作为复杂类型进行访问，因此可以使用下列方法，对架构扩展中的自定义数据执行 CRUD 操作：

- 资源 `POST` 方法可用于在新建资源实例时指定自定义数据。 请注意，**contact**、**event**、**message** 和 **post** 资源存在一个 [已知问题](known-issues.md#unable-to-create-a-resource-instance-and-add-schema-extension-data-at-the-same-time)，即需要使用 `PATCH` 操作创建架构扩展。
- 资源 `GET` 方法可用于读取自定义数据。
- 使用资源 `PATCH` 方法添加或更新现有资源实例中的自定义数据。
- 使用资源 `PATCH` 方法将复杂类型设置为 NULL，以删除资源实例中的自定义数据。

架构扩展示例：[使用架构扩展向组添加自定义数据](extensibility-schema-groups.md)

### <a name="schema-extensions-lifecycle"></a>架构扩展生命周期

当应用创建架构扩展定义时，系统会将该应用标记为该架构扩展的所有者。

所有者应用可以在 **状态** 属性上使用 PATCH 操作将扩展转换为生命周期中的不同状态。基于当前状态，所有者应用可以更新或删除扩展。架构扩展的任何更新始终只能累加且不能间断。

|状态 |生命周期状态行为 |
|:-------------|:------------|
| InDevelopment | <ul><li>创建后的初始状态。所有者应用仍然在开发架构扩展。 </li><li>在此状态下，在所有者应用注册的同一目录中的任何应用程序可以使用此架构定义扩展资源实例（前提是该应用对资源拥有权限）。 </li><li>仅所有者应用可以使用增量更改来更新扩展定义或将其删除。 </li><li>所有者应用可以将扩展状态从 **开发中** 更改为 **可用**。</li></ul> |
| 可用 | <ul><li>架构扩展可供任意租户中的所有应用使用。 </li><li>所有者应用将扩展设置为“可用”后，任何应用只需将自定义数据添加到扩展中指定的资源类型实例即可（只要应用拥有对相应资源的权限）。 新建实例或更新现有实例时，应用可以分配自定义数据。 </li><li>只有所有者应用，才能使用增量更改更新扩展定义。 任何应用都无法删除这种状态下的扩展定义。 </li><li>所有者应用可以将架构扩展状态从“可用”更改为“已弃用”。</li></ul> |
| 不推荐使用 | <ul><li>架构扩展定义不再可供读取或修改。 </li><li>任何应用都无法查看、更新、添加新属性或删除扩展。 </li><li>但是应用仍可读取、更新或删除现有扩展 _属性值_。 </li></ul> |

> **注意：** 其他开发人员从其他租户创建的架构扩展定义（标记为 `Available`）对所有开发人员可见（通过列出所有架构扩展）。 这不同于仅返回租户特定数据的其他 API。 另一方面，基于架构扩展定义创建的扩展数据是特定于租户的，并且只能由被显式授予权限的应用访问。 

### <a name="supported-property-data-types"></a>受支持的属性数据类型

在架构扩展中定义属性时，支持以下数据类型：

| 属性类型 | 备注 |
|:-------------|:------------|
| Binary | 最多 256 字节。 |
| Boolean | 不支持消息、活动和帖子。 |
| 日期时间 | 必须以 ISO 8601 格式进行指定。存储为 UTC 格式。 |
| 整数 | 32 位值。不支持消息、活动和帖子。 |
| 字符串 | 最多 256 个字符。 |

> **注意：** 不支持多值属性。

### <a name="azure-ad-directory-schema-extensions"></a>Azure AD 目录架构扩展

Azure AD 支持类似的扩展类型，在一些 [directoryObject](/graph/api/resources/directoryobject) 资源中称其为 [目录架构扩展](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)。你可以使用 Microsoft Graph API 来管理 [扩展属性定义](/graph/api/resources/extensionproperty)以及添加、获取、更新和删除这些扩展的属性中的 _数据_。

## <a name="permissions"></a>Permissions

还需要对特定资源执行读取或写入操作所需的相同[权限](./permissions-reference.md)，才能对相应资源上的任意扩展数据执行读取或写入操作。 例如，必须向应用授予 *User.ReadWrite.All* 权限，应用才能使用自定义应用数据更新登录用户配置文件。

此外，必须向应用授予 *Directory.AccessAsUser.All* 权限，才能创建和管理架构扩展定义。

## <a name="data-limits"></a>数据限制

### <a name="open-extension-limits"></a>开放扩展限制

以下限制适用于目录资源（**用户**、 **组**、 **设备**、 **administrativeUnit**、 **组织**）：

- 每个开放扩展最多可以包含 2KB 数据（包括扩展定义本身）。
- 应用最多可以为每个资源实例添加两个开放扩展。

以下限制将应用于 Outlook 资源（如“**邮件**”、“**事件**”和“**联系人**”）：

- 每个开放扩展存储在 [MAPI 命名的属性](/office/client-developer/outlook/mapi/mapi-named-properties)中，这是用户邮箱中的有限资源。 如需了解更多详情，请参阅 [openTypeExtension 资源类型](/graph/api/resources/opentypeextension)。

### <a name="schema-extension-limits"></a>架构扩展限制

应用程序最多可以创建五个 **架构扩展** 定义。

## <a name="known-limitations"></a>已知限制

有关使用扩展的已知限制，请参阅已知问题文章中的[扩展部分](known-issues.md#extensions)。

## <a name="extension-examples"></a>扩展示例

- [使用开放扩展向用户添加自定义数据](extensibility-open-users.md)

- [使用架构扩展向组添加自定义数据](extensibility-schema-groups.md)

## <a name="see-also"></a>另请参阅

- [Microsoft 365 域](/office365/servicedescriptions/office-365-platform-service-description/domains)

- [为 Microsoft 365 租户添加和验证域](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
